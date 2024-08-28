# Lovestruck: Ask To Work On Romance Dynamic Fix

The interaction to ask to work on a romance dynamic is unfortunately
broken. The interaction is supposed to work unless the tartget is in
a bad mood, or if the social context of the conversation is bad
(e.g. an Abhorrent or Boring discussion). In the checks for the
social context, the game mistakenly checks for the basic conversation
relationship bit (`relbit_SocialContext_Awkwardness_Casual`). This
is present for *every* conversation, meaning the interaction would
always fail. This is also the *only* interaction in the entire game
that checks for this specific bit, so it's likely a mistake.

This mod fixes the interaction by removing the misplaced
relationship bit.

Bug Report: [[LS] "Ask to Work On Romance Dynamic" always fails](https://answers.ea.com/t5/Bug-Reports/LS-quot-Ask-to-Work-On-Romance-Dynamic-quot-always-fails/m-p/13925150)
