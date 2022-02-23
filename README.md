<div align="center">
<h1>github-stats-stonks</h1>  
<h2>Where GitHub stats goes brrrr…</h2>  
  
![Stonks gif](https://i.giphy.com/media/YnkMcHgNIMW4Yfmjxr/giphy.webp)  
  
### Oh, so like that, you wanna fake your GitHub stats 🧐  
### Little cheater you are… But anyway, I'll help you 😁  
</div>

---

Have been tested with the following projects :  
+ [github-readme-stats](https://github.com/anuraghazra/github-readme-stats)  
+ [github-stats](https://github.com/jstrieb/github-stats)  
+ [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy)  
+ [metrics](https://github.com/lowlighter/metrics)  
+ *open an issue if it doesn't change anything on the one you're using, or if it's not among the above list*  

---

#### Summary :
[• Which stats can be faked ? 🤔](#what)  
[• How we can do that ? 🤩](#how)  
[• What are the limits ? 😒](#limits)  
[• I wanna contribute 🙋‍♂️](#contributing)  
[• FAQ (is it legal, would it nuke my account, …) 😣](#faq)  
[• Backstory of this repo, disclaimer and credits 🤝](#end)  

---

<a name="what"></a>**• Which stats can be faked ? 🤔**  
- [x] Commits  
Obviously commits can be faked ! This repo were mainly made for that. It's simple, works automatically and it's reliable  
- [ ] Stars  
Actually, yes, it's possible. But doing it needs alternative accounts, which is against GitHub rules  
- [ ] Pull requests  
Same as above  
- [x] Issues  
Since you can open issues by yourself, in *theory* it's possible. Didn't have worked on it yet, you can still open an issue if you need it (but not my priority yet)  
- [x] Profile views  
This one is pretty easy to fake, and can't be against GitHub rules because it uses a 3rd party service 😃  
- [x] Streak (see [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats) repo)  
Yes it works, depending of the frequency you chosen  
- [x] More… ?  
[Open an issue](https://github.com/EDM115/github-stats-stonks/issues/new)  

---

<a name="how"></a>**• How we can do that ? 🤩**  

It's pretty simple my tiger 😏 Just do follow the steps 👇  

1. Star this repo 🌟 (okay, this isn't mandatory, but it would help me so much 🥺 more stars means more motivation for me and I would do more projects. So please, consider starring this repo 🙏)  
2. ~~Fork it 🍴~~ Ehhhh no, forking this repo will not work 😌 Why ? Take a look [here](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/why-are-my-contributions-not-showing-up-on-my-profile#commit-was-made-in-a-fork) (TL;DR, commits on forked repositories doesn't count as yours until you do a pull request and that it's merged)
3. You need to click on that `Use this template` button
4. Once you're on your own version of my repo, go on `Settings → Secrets → Actions` and then click on `New repository secret`. You need to create two :
	1. Use `USERNAME` as name and your username as value
	2. Use `MAIL` as name and your mail adress as value  
Why are we using secrets ?  
	+ It's simpler, we don't have to modify dozen values on the code and we avoid in this way the risk to make a mistake
	+ It keeps your mail adress private, unless other repos
5. IT'S DONE 😝 Oh yeah but maybe you want it to runs at specific times… Well, here we go !
	1. Go on `.github/workflows` and click on the `stonks.yml` file
	2. Go at line №12 and modify the cron schedule Examples :  
	+ Every 15 minutes : `*/15 * * * *`
	+ Every hour : `0 * * * *`
	+ Each 4 hours on working days : `0 */4 * * 1-5`
	+ Twice a day every weekend : `0 8,20 * * 6,0`
	+ More examples at [`crontab.guru`](https://crontab.guru)
---

<a name="limits"></a>**• What are the limits ? 😒**  

Limits are numerous 😭 Here, I'm going to tell what limits exists and I'll also tell some stats :

Limits : 
+ Running times  
You might think that it can runs as much time as you want… 😏 Well **no** :smiling_face_with_tear:  
As example, you can't run it every second…
+ You can't do everything you want  
Things such as auto-follow and auto-stars are **not** allowed at all !  
  
Stats (without any modification at step 5) :  
Metric | Limit
----- | -----
Average runs per day | 80
Time to run the action | 15-30s

---

<a name="contributing"></a>**• I wanna contribute 🙋‍♂️**  

As you may have noticed (or not), the name of the commits aren't "normal". They can be :  
+ Quotes  
+ Sentences from movies / TV series / Video games  
+ Jokes  
+ Sarcastic things  
+ …  
You want to add more ? 😳  
[Open an issue](https://github.com/EDM115/github-stats-stonks/issues/new/choose), put `#quote` as title and type your sentence(s) that you wanna add to the project (if you have several, it's one per line). 99,9% of chances that it would be accepted
You see something wrong ? You have any problem with the script (non-working, …) ? You want to add a new functionality ?  
Once again, [open an issue](https://github.com/EDM115/github-stats-stonks/issues/new), describe shortly but surely what your issue is about in the title (examples : `Not working`, `Add auto-issue`, `Wanna stonks several URL's`, …) and be detailed on the description

---

<a name="faq"></a>**• FAQ (is it legal, would it nuke my account, …) 😣**  

+ Would it consume all my quota of Actions ?  
In case you didn't knew, we does actually have a [limit](https://github.com/settings/billing) on free GitHub plans. 2000 h/month, but it resets every 14 days  
Don't worry 😄 it uses 20-30 minutes per month, largely enough  

<div align="center">

![Free](https://telegra.ph/file/5b605e8d13cb67355702e.png)

</div>

+ Would it nuke my account ?  
Normally, no. What we have on this repo is safe. I didn't included anything that GitHub would use against you. Nevertheless, the owners of the stats things that appears on your profile might ban you… Don't abuse of the system !  
+ It works but my circle didn't change 🥺
Oh, so you're using anuraghazra’s repo ! Well, it's good but the commits don't have an enormous place on the way it calculates your rank  
Unless he changes the formula, I can't do anything for you  
+ Is it legal 🧐  
Yes it is 😄 But if you feel uncomfortable with this, or that you're a member of GitHub staff, you can reach me on Telegram : [**@EDM115**](https://t.me/EDM115)
+ It works, my contribution graph is stonksed but… it's disproportional and don't looks natural… 😓  
Well ! You can slow down the number of commits per day ([check step 5](#how))  
Now, if you're talking about **this** :  

<div align="center">

![Disproportionnal](https://telegra.ph/file/75c9854e505b70d51ba6b.png)  

</div>

Here's the solution :  
1. Go on each of your projects
2. Create a `TEMP` file (without any extension) at the root of your project
3. Create at the root a new file `.github/workflows/stonks.yml`
4. Copy the content of the `stonks.yml` present on this repository and paste it on the one of your project
5. That's all !
What we've done here ? We have basically boosted the number of commits in *another* of your repos 😇  
*Note :* if you didn't changed the cron schedule, the number of commits per day would looks like : `commits = number specified on .yml file × number of repos where you put it` *(me trying to looks like a mathematician 😭)*  

---

<a name="end"></a>**• Backstory of this repo, disclaimer and credits 🤝**  

This repo were inspired by ❌blablabla❌, noticed a huge amount of commits in ❌❌❌ repo, blablabla

Disclaimer : I'm not responsible, made for learning purposes, to know more about GH actions, ❌❌❌

Credits :
	random blabla ❌
