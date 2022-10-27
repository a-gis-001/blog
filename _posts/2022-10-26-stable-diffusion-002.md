---
title: "Stable Diffusion part 002"
date: 2022-10-26
---

![eye-it](https://user-images.githubusercontent.com/116606542/198154109-e9d769cc-1736-444c-ac3c-1beaef5b4f65.jpg)

## Test 1

Today I'm curious about styles in the Stable Diffusion UI. 
I created a photo style: "Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hirst". 
This was actually a mistake. I meant to not have the final author. So now we can see what Damien Hirst adds to the picture.

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 2,4,8,16,32,64,128
- Seed: 3233575213
- Size: 512x512

### "Euler a" with Photo Style + Damien Hurst

- Prompt: Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hurst, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hurst

Yes it is double. :) 

![xy_grid-0000-3233575213-Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hirst](https://user-images.githubusercontent.com/116606542/198148000-38bf6d05-34aa-42cf-9dd8-d898a98a9f61.jpg)

### "Euler a" with Photo Style

- Prompt: Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus

![xy_grid-0002-3233575213-Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus](https://user-images.githubusercontent.com/116606542/198150534-f315b3f2-c23a-408e-b2d2-34c4a7dc05f2.jpg)

## Test 2

Apparently the styles in Stable Diffusion UI just add it to the end of the prompt, so I had double prompts. Now I will just use my new photo style by itself but with a negative prompt so I don't get a bunch of cameras.

This one is interesting in that with lowef CFG Scale you just get stock photos of kids. It looks like this photo style really needs an actual subject.

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 4,8,16,24,32,40,48,64,80,96,112,128
- Seed: 3233575213
- Prompt: Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus
- Negative Prompt: camera
- Size: 512x512

### "Euler a"

![xy_grid-0000-3233575213-Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus](https://user-images.githubusercontent.com/116606542/198154217-ca09e827-8053-45c0-9b95-9144aa4eb869.jpg)


## Test 3

Now I'm tired of how long "Euler a" takes. I love DDIM. It's so fast. For 20 sampling steps, you get good stuff all day.  

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 8,16,24,32,40
- Seed: 3233575213
- Prompt: Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus
- Negative Prompt: 
- Size: 512x512

### DDIM

![xy_grid-0004-3233575213-Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels shar](https://user-images.githubusercontent.com/116606542/198164474-d05ec4a6-703a-4359-a9d1-095a806318a4.jpg)

I think the 20-30 corner with low steps is interesting. Let's look at that in detail in Test 5.

## Test 4

Now instead of "Starry night by Vincent van Gogh", I'm trying a simple "Woman" as the prompt.

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 8,16,24,32,40
- Seed: 3233575213
- Prompt: Woman, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus
- Negative Prompt: 
- Size: 512x512

### DDIM

![xy_grid-0003-3233575213-Woman, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus](https://user-images.githubusercontent.com/116606542/198164555-cb107a77-040f-4e01-9a98-959c85b223e2.jpg)

## Test 5

There's some cool stuff in the 20-30 range and low step count. Let's investigate!

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 8,16,24,32,40
- Seed: 3233575213
- Prompt: Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus
- Negative Prompt: 
- Size: 512x512

### DDIM

![xy_grid-0005-3233575213-Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels shar](https://user-images.githubusercontent.com/116606542/198164611-741d2719-fa92-4194-a399-435f583dd91d.jpg)

## Bonus Buys

### Puff weed is your name

This was one random variant that popped up that looked cool.

![00001-3298187535-Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hirst](https://user-images.githubusercontent.com/116606542/198152693-a152f8eb-86a0-426c-8423-52d4019325b0.png)

### Euler a + low steps + random seed

I accidentally ran Euler a with low step counts with a random seed for both "Starry night by Vincent van Gogh" and  "Woman" as the prompt.

#### Prompt: Starry night by Vincent van Gogh

![xy_grid-0001-3694350114-Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels shar](https://user-images.githubusercontent.com/116606542/198155203-47af9001-7bd8-4eed-adb2-9b9663b10e88.jpg)

#### Prompt: Woman

![xy_grid-0002-3520326817-Woman, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus](https://user-images.githubusercontent.com/116606542/198155762-d9fd66a2-a774-4ab7-a1ae-45c6b70b465b.jpg)

#### Prompt: World's Strongest Man

![xy_grid-0006-3233575213-World's Strongest Man, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus](https://user-images.githubusercontent.com/116606542/198174675-0e019c1b-9a36-44e9-a62e-7c6e7cb33dfd.jpg)
