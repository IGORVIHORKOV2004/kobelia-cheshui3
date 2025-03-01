# kobelia-cheshui3
kobelia cheshui2
import  tkinter
import pygame


master = tkinter.Tk()
canvas = tkinter.Canvas(master, bg='white', height=600, width=600)
for event in pygame.event.get():
    if event.type == pygame.QUIT:
        game_exit = True
    if event.type == pygame.KEYDOWN:
        if event.key == pygame.K_w:
            loc_y += 25
        if event.key == pygame.K_s:
            loc_y -= 25
        if event.key == pygame.K_a:
            loc_x -= 25
        if event.key == pygame.K_d:
            loc_x += 25


canvas.pack()
master.mainloop()
