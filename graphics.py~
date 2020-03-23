import pygame as pg
pg.init()
screen = pg.display.set_mode((800,600), pg.HWSURFACE)

scale = 32
for i in range(0,12):
	for j in range(0,12):
		if (i+j)%2 ==0:
			pg.draw.rect(screen,(255-i*20,255-j*10,i*20),(scale*i,scale*j,scale,scale))
		else:
			pg.draw.rect(screen,(255,255,255),(scale*i,scale*j,scale,scale))
	
active = True
while active:
	pg.event.pump()
	keys = pg.key.get_pressed()
	if(keys[pg.K_ESCAPE]):
		active=False
	pg.display.flip()
	pg.time.Clock().tick(18)
pg.quit()

