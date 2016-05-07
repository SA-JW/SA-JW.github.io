---
title:  MICROBIT TUTORIALS
layout: post
author: sam.woodroff
permalink: /-microbit-tutorials/
source-id: 1bjrGeJ3H5OXMpgXbkR16WxQN4VcmTG_TbvkjD-Oz6i0
published: true
---
BBC MICROBIT TUTORIALS

In my ninth blog post, named BBC MICRO:BITS, I began to talk about some of the handy tutorials that guide you through a script and help you learn the basics. In our most recent IT lesson, our teacher handed out a code kingdoms "cook book" via our google classroom page. Listed in this document were guides on each of the Javascript tutorials with learning outcomes clearly defined, plus an extension task if you wanted to expand your knowledge. In the first tutorial, the learning outcome was essentially to get you to write a simple code and understand how it works. At the beginning, when we were first introduced to Microbit, I had already completed that tutorial and I learnt that programmes work in a very specific way, so you have to be very precise with your code.  In the second tutorial, the extension task really helped me. The idea of “mood swing” is when you tilt the microbit in a certain direction, a different face appears - the extension task was to make the LED brighter when happy and lower when sad. I began by adding a change brightness block like this in my code:

	if (microbit.tiltY < 2) {

			

			microbit.draw(Pattern("01010.01010.00000.01110.10001"));

			microbit.brightness = 125;

I did the same for a happy face only with increased brightness. When I ran the code there was some kind of error that didn't let it do so. I then realised that I’d have to set the brightness at the beginning. This is what my code turned out as:

	/* When the BBC micro:bit runs   */

function onStart(  ) {

	microbit.brightness = 200;

	while (true) {

		

		if (microbit.tiltY == 2) {

			

			microbit.draw(Pattern("01010.01010.00000.00000.11111"));

			microbit.brightness = 200;

			

		}

		

		if (microbit.tiltY < 2) {

			

			microbit.draw(Pattern("01010.01010.00000.01110.10001"));

			microbit.brightness = 125;

			

		}

		

		if (microbit.tiltY > 2) {

			

			microbit.draw(Pattern("01010.01010.00000.10001.01110"));

			microbit.brightness = 255;

			

		}

		

		

	}

	

	

}

I wonder what our next challenge will be? 

