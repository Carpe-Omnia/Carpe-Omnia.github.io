---
layout: post
title:      "React Redux Portfolio Project"
date:       2019-03-23 23:21:05 +0000
permalink:  react_redux_portfolio_project
---


So I've been working on this portfolio project for a little while now. I think it's kinda cool. Basically the whole idea is that it's based on the user never having to reach for the mouse. Turns out this wasn't quite as easy to implement as I had hoped. 
The actual core functionality of the site is not that interesting. Users can make accounts, log-in, log-out, write jokes (with hidden punchlines revealed via hotkey events), edit their profile, and send messages back and forth. The cool part is that the entire document is hooked up with an event listener that monitors keystrokes, which is often useful in place of a cursor. You can navigate side-to-side between components using the arrow keys, and almost every interactable element has been assigned a hotkey. I created a React.Component specifically for adding hotkey's and hotkey-helpers to elements, which makes their usage significantly easier. They can be used like;
`<button type="submit" value="submit" id="submit_joke" >
      Submit <Hotkey text="j" click={true}/>
 </button>` 
The above snippet of code binds the hotkey 'j' to that particular element, without needing to do anything else. And the best part is that because of the way React works, this element can share that hotkey with many others as long as they aren't being rendered at the same time. The hotkey helpers also automatically disappear on mobile, as their presence would be incrediblly irritating. In all honesty I think some of the components I've written here might be more useful as a mini-library than as part of this particular app.  
I don't know how long these blog posts are supposed to be, so I'm just going to cut this off because I want to move on to the code review. 

