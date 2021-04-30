---
layout: post
title:      "Hibiscus Lovers - RubyonRails app"
date:       2021-04-30 16:33:40 +0000
permalink:  hibiscus_lovers_-_rubyonrails_app
---

This is my third project for Flatiron self-pace software engineering program. I’m so pleased that I have just done ⅔ of the journey. 2 more projects to go and I’m ready to join the IT workforce. This is called “Hibiscus Market” by which all hibiscus lovers from all over the world can use to share as well as sell and buy hibiscus seeds. Yes, I’m still so obsessed with the beauty of this kind of tropical gem. The blooms are something out of this universe. There are just so many colors and patterns. Especially the most fascinating thing is when we cross pollinate them the offspring will have unpredictable colors. I have bought around 100 seeds and had them germinated in my seed starting kit. It is such an ease to watch them growing up every day. I hope they all will make it to become strong and healthy plants. Back to my project, it is a ruby on rails app. There are session, user, cultivar, sale and order models. Together they help to make this app operating like a mini commercial website (selling and buying things). A user can sign up via a regular way or can use login with a github account. This login with github step was such a pain in the butt. I was able to have it done smoothly but when I reviewed it before having it submitted, there was a mismatch url issue. Even though I spent almost a day checking the registered and redirect urls, I was desperate to have it work again. TCs could not figure out this problem either so I gave up. I wanted to use facebook login instead but FB asks users to have url policy stuff blah blah blah and it costs money. So I decided to  go with google oauth2  strategy. Based on what people said on stack overflow, the miss match issue just happens to github but not google. When I read through the README I found out this line of code:

OmniAuth.config.full_host = Rails.env.production? ? 'https://domain.com' : 'http://localhost:3000' 
I applied it to my project and a mismatch issue was solved but another issue emerged: “csrf detected”. To be honest I did not know what it meant. I kept googling and a guy suggested to use this line of code to add in omniauth.rb file 
provider_ignores_state: true
It works! Hooray. Finally!!!

This project took me almost 3 months to finish even though it is kind of similar to the Sinatra app. The self-pace program is no joke when my biggest enemy is the tardiness. 2 more projects to go. I need to push myself harder to finish this program by summer. 




