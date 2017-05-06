---
title: Second Codecademy Lesson - Pyg Latin
layout: post
author: sam.woodroff
permalink: /second-codecademy-lesson---pyg-latin/
source-id: 1nsATIlTnbaf4rmjgMN00dJwRWLt7gq2F1mmkCnau5WU
published: true
---
Last lesson I began a Codecademy lesson called Pyg Latin, which is a calculator that takes the first letter of a word, adds it to the back and adds ay to the back, so pizza would become izzapay. Quite simply the way that you do it is creating a variable that contains the string 'ay'; then creating a raw input that allows the user to enter the word that the want translated; then creating a statement that checks have they actually typed in a word and using is.alpha, checking if the word has numbers in it and then displaying an error message; then creating a variable that contains the first letter of the word you typed in and then adding up the variables together. This is what my code looked like:

pyg = 'ay'

original = raw_input('Enter a word:')

word = original.lower()

if len(original) > 0 and original.isalpha():

    print original

else:

    print 'empty'

    

first = word[0]

new_word = word[1:len(new_word)] + first + pyg 

 

