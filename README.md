#         Artem Oleynikov
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

## Gallery:

![Image](ArtemOleynikov.github.io/docs/assets/images/1k8TBeuIuYiBwBfIscJ8F1ciznAQ4IqqsGvAa7xBJHPNJWxstm5LE1RdN7SbzL4uwkZxew.jpg)

![Image](ArtemOleynikov.github.io/docs/assets/images/bUTT3JhRnZcyKMyKAG26TS7LNkCbJ1Cyd5vVLbfVN3LkVyxRWjRr4sMfDVpPtGIcC6x6QQ.jpg)

![Image](ArtemOleynikov.github.io/docs/assets/images/CvPAlE1RplsoTV0NhwmUsagR42F8W8SiS8YY3cYGdZsGczW_Q4e3uqshYFiS0bw9-1B72qM0.jpg)

### Socials: 

Questions, remarks, constructive critisism? 
Contact me on [Telegram](https://t.me/artem_oleynikov) or on [Instagram](https://support.github.com/contact) if you're more of a visual type.
