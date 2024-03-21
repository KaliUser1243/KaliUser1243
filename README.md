  I am <b>KaliUser1243</b> and I am a young programmer,
I focus on using Python, and Bash. I love to do ethical hacking with the two.

  I use Ubuntu 22.04.3 and 23.10 LTS. I also have a Raspberry Pi running Kali Linux.
Along with that, I am learning to use WSL on Windows 11 Pro on a MiniPC.
I LOVE to code, I am also actively trying to build a robot with a Raspberry Pi. As I
said, I am still young and still learning evrything.

If you want, here is a Python script that uses pygame,


import pygame
import sys

# Initialize Pygame
pygame.init()

# Set the dimensions of the window
WINDOW_WIDTH, WINDOW_HEIGHT = 500, 500
window = pygame.display.set_mode((WINDOW_WIDTH, WINDOW_HEIGHT))
pygame.display.set_caption("Pygame Window")

# Set colors
WHITE = (255, 255, 255)
RED = (255, 0, 0)

# Define the rectangle's properties
rect_width, rect_height = 50, 50
rect_x, rect_y = (WINDOW_WIDTH - rect_width) // 2, (WINDOW_HEIGHT - rect_height) // 2
rect_velocity = 5

# Create a rectangle sprite
rectangle = pygame.Rect(rect_x, rect_y, rect_width, rect_height)

# Main loop
running = True
while running:
    window.fill(WHITE)  # Fill the window with white color

    # Event handling
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # Move the rectangle with arrow keys
    keys = pygame.key.get_pressed()
    if keys[pygame.K_LEFT] and rectangle.left > 0:
        rectangle.x -= rect_velocity
    if keys[pygame.K_RIGHT] and rectangle.right < WINDOW_WIDTH:
        rectangle.x += rect_velocity
    if keys[pygame.K_UP] and rectangle.top > 0:
        rectangle.y -= rect_velocity
    if keys[pygame.K_DOWN] and rectangle.bottom < WINDOW_HEIGHT:
        rectangle.y += rect_velocity

    # Draw the rectangle
    pygame.draw.rect(window, RED, rectangle)

    # Update the display
    pygame.display.update()

# Quit Pygame
pygame.quit()
sys.exit()

You can use the arrow keys to move around!

Thank you for visiting this profile!
Have A Good Day!
