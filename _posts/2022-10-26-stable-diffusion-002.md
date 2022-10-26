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

Now I'm tired of how long "Euler a" takes. I love DDIM. It's so fast. For 20 sampling steps, you get good stuff all day. So I'm going 

### Parameters

- CFG Scale: 5,10,15,20,25,30
- Steps: 8,16,24,32,40
- Seed: 3233575213
- Prompt: Starry night by Vincent van Gogh, Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus
- Negative Prompt: 
- Size: 512x512

### DDIM

## END

![00001-3298187535-Professional photography, bokeh, natural lighting, canon lens, shot on dslr 64 megapixels sharp focus, by Damien Hirst](https://user-images.githubusercontent.com/116606542/198152693-a152f8eb-86a0-426c-8423-52d4019325b0.png)

