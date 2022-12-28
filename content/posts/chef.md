---
title: "Chef"
date: 2022-12-27T21:17:05-05:00
draft: false
---

## Introduction

_Chef_ was an experimental case-based planning project developed by Kris Hammond. It used the domain of cooking as a way to explore the use of case-based reasoning in planning. A "micro" version of _Chef_ can be found in _Inside Case-Based Reasoning_[^icbr] (ICBR).

The case study in ICBR considers plan adaptation, failure prediction, and failure repair. A recipe for stir-fry beef and green beans is adapted for beef and broccoli, but the broccoli comes out soggy, because it has been cooked in too much broth from the beef. The suggested repair is to use less broth.

Will ChatGPT come close to this in the recipe domain?

## ChapGPT's Version

As expected, asking for a beef and beans stir fry recipe is easy. There are a lot of recipes on the Internet. When I asked to adapt the recipe to use broccoli instead of green beans, it basically just replaced the beans for broccoli. I then asked:

> Ok, I tried that, but the broccoli was soggy. Do you have any idea why?

It came up with three reasons, all fairly reasonable:

> 1. You may have overcooked the broccoli. Broccoli should be cooked just until it is tender-crisp, so it's important not to overcook it. If you cook it for too long, it can become soggy and lose its texture.
> 2. You may have added too much liquid to the pan. If you added a large amount of sauce or other liquid to the pan, it could have caused the broccoli to become soggy.
> 3. You may have used a pan that was too small. If the pan you used was too small, the vegetables may have been crowded and steamed rather than stir-fried.

I asked it to adjust the recipe with this in mind, and it replied:

> To help prevent the broccoli from becoming soggy, be sure to cook it just until it is tender-crisp and use a minimal amount of sauce or other liquid. Make sure to use a pan that is large enough to allow the vegetables to cook evenly, and be sure to stir the vegetables frequently while cooking to ensure even cooking.

In a different session (theoretically without a memory of the first interaction), I asked, after it gave me a beef-and-beans recipe;

> If I adapted this to use broccoli instead of beans, is there anything I need to worry about or do differently?

It gave three answers:

> 1. Cook the broccoli slightly longer than the green beans. Broccoli tends to take a little longer to cook than green beans, so you may need to add an additional 1-2 minutes of cooking time.
> 2. Cut the broccoli into small, bite-sized pieces. This will help it cook evenly and make it easier to eat.
> 3. Be careful not to overcook the broccoli. Overcooked broccoli can become mushy and lose its crunch, so aim for al dente texture. You can test for doneness by piercing a piece of broccoli with a fork. If it is tender but still has some firmness, it is done.

## Commentary

### Bullshit detected

1. In the second recipe, it suggests cooking the broccoli longer, but this is just not the case. It's very confident of its answer, though!
2. Cutting the broccoli into "bite-size pieces" will definitely make this recipe worse, although its suggest to not overcook it is solid.


### Missed opportunities

1. The "you may have added too much liquid to the pan" reason is not the case; the liquid was present from the beef, and it had no sense of that.
2. It certainly did the least amount of work (as it were) in adapting the recipe in the first case; assuming that it was (in some sense) confident in the first recipe, it didn't consider what adaptations would be necessary for the substitution.

### DANGER, WILL ROBINSON

Of course, I asked it to substitute various poisonous mushrooms. It wouldn't give me a recipe for death cap mushrooms, but was perfectly fine with false parasol mushrooms. These, according to ChatGPT, are "also known as shiitake mushrooms," both bullshitty and dangerous.


[^icbr]: Riesbeck, Christopher and Roger Schank. (1998). Inside Case-Based Reasoning. Psychology Press. A version can be checked out from the [Internet Archive](https://archive.org/details/insidecasebasedr0000ries/page/164/mode/2up). The micro version of _Chef_ is on page 164.
