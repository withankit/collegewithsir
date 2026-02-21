import pygame
import random
import sys

# Initialize pygame
pygame.init()

# Screen size
WIDTH = 600
HEIGHT = 400
BLOCK = 20

screen = pygame.display.set_mode((WIDTH, HEIGHT))
pygame.display.set_caption("Snake Game")

# Colors
white = (255, 255, 255)
black = (0, 0, 0)
green = (0, 255, 0)
red = (255, 0, 0)

clock = pygame.time.Clock()
font = pygame.font.SysFont(None, 35)

def draw_snake(snake_list):
    for block in snake_list:
        pygame.draw.rect(screen, green, [block[0], block[1], BLOCK, BLOCK])

def message(text, color):
    msg = font.render(text, True, color)
    screen.blit(msg, [WIDTH / 6, HEIGHT / 3])

def game():
    game_over = False
    game_close = False

    x = WIDTH / 2
    y = HEIGHT / 2

    x_change = 0
    y_change = 0

    snake_list = []
