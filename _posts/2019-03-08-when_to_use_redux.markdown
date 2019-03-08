---
layout: post
title:      "When to use Redux"
date:       2019-03-08 21:25:48 +0000
permalink:  when_to_use_redux
---


You might be confused about when to use Redux over React. This entirely depends on the complexity of your state! 

Before we can answer that question, we need to answer this one: What the heck is a state?!

A state can be many things such as what the user sees (the data), fetching data, the URL the user sees, items selects on the page, etc.

In an application where data is shared across components, it is unclear where the state should live. In React, it is required that state lives in a parent component in order to be shared amongst siblings. 

Redux solves this problem by keeping the state in a store in which any component can access. Therefore, each component gets the exact state in needs at all times! 

So, if  you application requires state management across components, Redux is the way to go. 

