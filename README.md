# hello
import sys
import pygame

class AllenInvasion:

    def __init__(self):
        pygame.init()
    
        self.screen = pygame.display.set_mode((1200,800))
        pygame.display.set_caption("Allen Invation")
    
    def rin_game(self):
    
        while True:
        
            for event in pygame.event.get():
                if event.type == pygame.QUIT:
                    sys.exit()
            
                pygame.display.flip()
if __name__ == '__main__':
    ai = AllenInvasion()
    ai.run_game()
