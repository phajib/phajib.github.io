---
layout: post
title:      "An Empty File only brings Encouragement to what You can Transform it to Be"
date:       2019-04-15 06:54:32 +0000
permalink:  an_empty_file_only_brings_encouragement_to_what_you_can_transform_it_to_be
---


Prior to creating this gem, the labs that I completed provided the platform for this project. It has created a foundation in understanding Object Oriented Programming. When you have embraced OOP everything else follows and it begins to flow like milk entering a glass, filling to the top, much like your mind becomes full but never stops to yearn for more. The complexity of Ruby is wonderful yet simple and clean. There is something about Ruby that makes learning to code a welcoming experience.

![](https://data.whicdn.com/images/47006585/large.png)

Being a lover for sneakers, this inspired me to share the beauty of the Air Max. This gem scrapes a particular website that talks about the history of the Nike Air Max shoe. That scraped data is placed within a menu where the user selects a particular shoe to read about that shoe. This gem was formed with the help of the `nokogiri` and `open-uri` gems.

***Air Max CLI***

As daunting as it may seem to type the those few commands `bundle gem <gem_name>` you've just taken the first step in building your gem. In this case I created one that spoke of the history of the Nike Air Max, `bundle gem air_max`. Bundler created a basic structure for my gem, a *bin*, *lib* and my *air_max* folders. It also creates other core files which will assist in running your gem. I am now in and there's no turning back, welcome to my *Comman Line Interface* Data Gem Portfolio Project.

After the structure of my gem was made, I needed to create an executable file that would run the CLI. In the `./bin` folder I created `air_max` file, this is my executable file. Within that file I needed to tell my bash terminal that I am creating a gem in Ruby, `#!/usr/bin/env ruby`. Within that file I simply outputted a simple test, `puts Have a Nice Day!` and in terminal I executed the file by typing `./bin/air_max` and as expected it printed out *Have a Nice Day!*

Next, I needed to create the body of the gem. I created four main classes, three of which lived in the `.lib/air_max` folder and the other in the `./lib` folder. Within `./lib/air_max` was `air.rb`, `cli.rb`, and `scraper.rb`. In `./lib` the fourth class was `environment.rb`. The `environment.rb` file is what sets the environment for the gem. Within the class I needed to `require` other gems that would assist in the operation of the other files. Three important gems that were crucial were `pry`, `nokogiri`, and `open-uri`. For the files to interact with each other the three other files,`air.rb`, `cli.rb`, and `scraper.rb` needed to be within the environment file through the `require_relative`method.


***Scraper***

Instead of searching for information to type about the History of Air Max, there is a much better tool to use, that is *Scraping*. Scraping allows us to select certain parts of a website and utilize that data in to the CLI. Remember how we can use certain gems to helps us in creating this gem, well `nokogiri` and `open-uri` gems are key players. Both gems allows us to dissect a chosen website and see how we can utilize it's HTML to retrieve the data we need. Once we have found the data, we need to store it so it can be used within the gem.


***Air***

The `air.rb`'s duty is to store the retrieved data from our `scraper.rb`. We have a class variable array that holds all the data we scraped. Having instance variables in the attr_accessor allows them to be used in our other files, mainly the `cli.rb` file. We have our `shoe_name` and `description` instance variables that hold the name and information about each Air Max shoe.


***CLI***

The *Command LIne Interface* controller is what provides interaction between the user and the code. This class sets out a menu and input system through three main methods, `menu`, `shoe_list`, and `am_list`. Once the file gem is executed using `./bin/air_max` command in the terminal, the CLI begins with a menu together with a listing of Air Max shoes ranging from 1978 to 2019. The user is then asked to select a shoe by inputting a number between 1-27 and the corresponding information is displayed. The menu format is looped until the user quits by typing in `exit`.


After consuming many glasses full of information, my mind conformed with my fingers and become one with the keyboard. I suprised myself that I was able to transform all that knowledge to this gem, **Air Max**.

![](https://sneakernews.com/wp-content/uploads/2019/02/nike-have-a-nike-day-release-dates.jpg)
