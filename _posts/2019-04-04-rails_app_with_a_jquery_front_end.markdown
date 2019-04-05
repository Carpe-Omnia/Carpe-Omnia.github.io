---
layout: post
title:      "Rails App with a jQuery Front End"
date:       2019-04-05 01:20:10 +0000
permalink:  rails_app_with_a_jquery_front_end
---


Not really that much to say about this one. It's shockingly similar to my final rails project, which already made some use of jQuery. The important difference here is that users can reply to messages without exiting the screen they're already in, which is pretty much the core of what I was going for. I was also thinking about how how cool it would be if Rails could somehow serve views, but do it through an API rather than the traditional way. I ultimately decided against pursuing this though, because it's really not that good of an idea. Whatever load time you saved on initial load-up would ultimately be paltry compared to the extra time spent loading views instead of just data. It would also be tricky to maintain functionality of the views across stringification. I think the current paradigm of JS front-end with rails backend that handles data persistence is probably the best solution. 
