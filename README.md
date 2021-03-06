# Artem Oleynikov
Navigating my way through a career in IT, a myriad of hobbies and just life in general

My mission is simple: discover, try and share different practices that make the journey more enjoyable, interesting or efficient

## Bit of the week: 

### _We suffer more in imagination than in reality_ - Seneca

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

### Socials: 
Questions, remarks, constructive critisism? 
Contact me on [Telegram](https://t.me/artem_oleynikov) or on [Instagram](https://www.instagram.com/suchacrookedvulture/) if you're more of a visual type.
