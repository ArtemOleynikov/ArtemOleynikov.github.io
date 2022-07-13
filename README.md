# Artem Oleynikov
Navigating my way through a career in IT, a myriad of hobbies and just life in general

My mission is simple: discover, try and share different practices that make the journey more enjoyable, interesting or efficient

## Bit of the week: 

###_We suffer more in imagination than in reality_ - Seneca

## Code snippet of the week: 

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for
```markdown

Let's visualize airports in R

`library(jsonlite)
library(dplyr)

# globejs 
airports <- fromJSON("https://raw.githubusercontent.com/jbrooksuk/JSON-Airports/master/airports.json")

# create a dataframe key of size to colors
sizecolors <-
  data_frame(size = c("small","medium","large"),
             color = c("lightblue", "gold","firebrick"))

airports <-
  airports %>%
  # some of the data is missing lat and lon
  filter(!is.na(lat) & !is.na(lon)) %>%
  # join with colors
  left_join(sizecolors)

globejs(lat = airports$lat, 
        lon = airports$lon,
        color = airports$color)`

```
Try it for yourself! 

## Book of the month: 

 [Meditations](https://www.gutenberg.org/ebooks/2680) by Emperor of Rome Marcus Aurelius 

## Gallery:

![Image](https://scontent-bru2-1.cdninstagram.com/v/t51.2885-15/292534819_740584607272464_7675952729522134041_n.webp?stp=dst-jpg_e35&_nc_ht=scontent-bru2-1.cdninstagram.com&_nc_cat=100&_nc_ohc=zCfaKwCu8DUAX-Bvloh&edm=ALQROFkBAAAA&ccb=7-5&ig_cache_key=Mjg3OTg3MjI4MzYzNzY1NTMzNQ%3D%3D.2-ccb7-5&oh=00_AT9GxqrQkme2aJboWPRZDkjfo4f6VvI_ETJBaz-2byTH_A&oe=62D5FD3E&_nc_sid=30a2ef)
![Image](https://scontent-bru2-1.cdninstagram.com/v/t51.2885-15/238191731_182308683852790_4297461498432111308_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent-bru2-1.cdninstagram.com&_nc_cat=110&_nc_ohc=xckRoKOAuW8AX9KSco6&edm=ALQROFkBAAAA&ccb=7-5&ig_cache_key=MjY0MjA5NTQwNDAzNDUwMDk3NA%3D%3D.2-ccb7-5&oh=00_AT-YkJVWbdL3WLJtLS6ee2BQ-7g-UJqXYCaKHCsB-pzZxQ&oe=62D69B57&_nc_sid=30a2ef)
![Image](https://scontent-bru2-1.cdninstagram.com/v/t51.2885-15/107872813_139134437825483_5356810640007085497_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent-bru2-1.cdninstagram.com&_nc_cat=111&_nc_ohc=8hS6L0hUODkAX-ZJCr9&edm=ALQROFkBAAAA&ccb=7-5&ig_cache_key=MjM1MTUzMTIxMzY4ODYwODM5Mg%3D%3D.2-ccb7-5&oh=00_AT83ry09yoaA-eQY9rWKJhEL3dof0w8jprfagwPWjijYhQ&oe=62D6E2C0&_nc_sid=30a2ef)

### Socials: 

Questions, remarks, constructive critisism? 
Contact me on [Telegram](https://t.me/artem_oleynikov) or on [Instagram](https://support.github.com/contact) if you're more of a visual type.
