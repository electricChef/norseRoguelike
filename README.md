import random, math, pygame
from pygame.locals import *

names = ["Algot",   "Alrik", "Andren",
         "Aren",	"Arvid",	"Ask",
"Assar",	"Atle",	"Axel",
"Bjorn",	"Boden",	"Britt",
"Canute",	"Christoffer",	"Dahl",
"Dane",	"Daube",	"Davin",
"Delling",	"Donar",	"Dyre",
"Ebbe",	"Eero",	"Egil",
"Eilert",	"Elof",	"Elvis",
"Ensio",	"Eric",	"Erik",
"Erling",	"Esbern",	"Eskil",
"Espen",	"Flanders",	"Frey",
"Geir",	"Gerik",	"Gimli",
"Gunnar",	"Gunner",	"Hakan",
"Halden",	"Haldis",	"Hallmar"]

titles = ["the Bold", "Shieldbreaker", "Whitebeard", "Hornblower",
          "the Black Goat", "the Knight of Roses", "Bloodcloak",
          "Swiftblade", "Coldhands", "Halfhand", "the Weeper", "Stoneface",
          "Icehammer", "of Rock Fjord", "of Windy Crag", "of Stormy Isle",
          "of Gull Roost", "of Walrus Bay"]

shipNames = []
crew = []

'''pygame.init()
screen = pygame.display.set_mode((150, 150))
pygame.display.set_caption('Basic Pygame program')
background = pygame.Surface(screen.get_size())
background = background.convert()
background.fill((250, 250, 250))
font = pygame.font.Font(None, 12)
text = font.render("Hello There", 1, (10, 10, 10))
textpos = text.get_rect()
textpos.centerx = background.get_rect().centerx
background.blit(text, textpos)
screen.blit(background, (0, 0))
pygame.display.flip()'''

print "Hello"
name = raw_input('What is your name? ') + " " + titles.pop(random.randint(0, len(titles)-1))
print "Hello" + name
print "You are the leader of a band of adventurers"
print ""
print "These are your loyal cohorts:"

for x in range (0, 6):
    crew.append(names.pop(random.randint(0, len(names)-1)) + " " + titles.pop(random.randint(0, len(titles)-1)))
    print crew[x]

print ""
print "Choose a god to worship"
print "(a) R'hollor, Lord of Light and Fire"
print "(b) Gaea, Goddess of Earth and Nature"
print "(c) Wendigo, Haunter of the Tundra"
print "(d) Odin Stormfist"
print "(e) Father Dagon, King Beneath the Waves"
print "(f) Death, The Hooded One"
god = raw_input()
if god in ["a"]:
    print "You have chosen R'hollor"
elif god in ["b"]
