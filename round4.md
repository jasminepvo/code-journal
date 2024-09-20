### Day 1: September 9, 2024 - Monday

#### Todays's Progress

✅ Completed 2 codewars problem <br>
✅ CSSBattle <br>
✅ UI for 75Hard Tracker

#### Thoughts

- Here we go again. Truth is, I prioritized my job over lifetime learning and consistency. As a new developer who just landed my first job in tech, which has been a dream of mine, I felt as if I owed my full time commitment and duty to performing as best as possible in my new role, since I was also making the most I've ever made in my life. Since then, i've learned tremendously and made an impact in that position which led me to fulfill even bigger dreams. I became a cofounder and frontend engineering lead, working with the most amazing programmer / friend currently who's doing big things at Google. I learned so much when it came to AI, backend, cloud, project mangement, marketing and all other responsiblities that come with a startup. I don't regret anything. Just looking forward to getting back to consistently coding/learning!
- Codewars was a good refresher on .replace() and regex
<img width="1264" alt="Screenshot 2024-09-09 at 5 20 45 PM" src="https://github.com/user-attachments/assets/343f6079-97a6-414c-8708-95a00cba980d">
<br><br>

- Also can't forget about my daily css battle. A heart is just 2 circles overlapping a square at 45deg.
<img width="1264" alt="Screenshot 2024-09-09 at 8 04 22 PM" src="https://github.com/user-attachments/assets/723af27e-fee4-470c-97a3-1acb6f005ba0">

---

### Day 2: September 10, 2024 - Tuesday

#### Todays's Progress

✅ Daily CSSBattle <br>
✅ Daily codewars

#### Thoughts

- First time getting 100% right!!! Such a little win but made me so happy.
- <img width="1264" alt="Screenshot 2024-09-10 at 11 56 03 PM" src="https://github.com/user-attachments/assets/8cad5662-d250-41ea-9617-4bf11116160c">
- First attempt <img width="1212" alt="Screenshot 2024-09-11 at 12 13 41 AM" src="https://github.com/user-attachments/assets/a4fd2d7d-5f17-4659-9495-c6d5514c4629">
- But then I realized I could clean it up and refactored
```
  function finalGrade (exam, projects) {
  if(exam > 90 || projects > 10) return 100;
  if(exam > 75 & projects >= 5) return 90;
  if(exam > 50 & projects >= 2) return 75;
  return 0;
}
```
---

### Day 3: September 11, 2024 - Wednesday

#### Todays's Progress

✅ Daily codewars

#### Thoughts

- Good ole palindrome question :)
- <img width="1712" alt="Screenshot 2024-09-11 at 4 46 51 PM" src="https://github.com/user-attachments/assets/47efe5d5-e699-4087-93eb-21e99a4195cd">
- Ahh after seeing other solutions, I realized this would have been better, or using a ternary operator
-
```
  function isPalindrome(x) {
    return x.toLowerCase().split('').reverse().join('') == x.toLowerCase()
  } 
```

---

### Day 4: September 12, 2024 - Thursday

#### Todays's Progress

✅ Daily CSSBattle


#### Thoughts

- Here is my solution for today! However, it made me think it also would have been possible to reflect the top / bottom div on the x axis as well.
- <img width="1679" alt="Screenshot 2024-09-12 at 2 50 47 PM" src="https://github.com/user-attachments/assets/aa0282ab-bd29-4406-897e-e1a4050755ec">
- After diving deeper into CSS reflections, I learned it's possible with 2 different ways
  - 1. transform: scaleX(-1) (SOURCE:https://css-tricks.com/snippets/css/flip-an-image/)
  - 2. -webkit-box-reflect: <direction> <offset> (SOURCE:https://webkit.org/blog/182/css-reflections/)
   
- Although these CSS battles have primarily been shapes sized/ordered differently, it's definitely made me realize there are some cool CSS properties that I'm not as familiar with! It's good to hone in on my skills.

---

### Day 5: September 19, 2024 - Thursday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle

#### Thoughts

- Took a few days off because my family drove in town (26hrs) so I wanted to cherish the moments with them.
- Picking back up as usual though! Today's codewars I could see the refactored solution initially but it still always helps me to write pseudocode first.


Initial:
```
function sumStr(a,b) {
  //convert string to num
  let num1 = a === '' ? 0 : Number(a);
  let num2 = b === '' ? 0 : Number(b);

  //sum a and b
  let sum = num1 + num2;

  //return sum as string
  return sum.toString();
}
```
Refactored:
```
function sumStr(a,b) {
  return String(Number(a) + Number(b));
}
```

- My thoughts on this CSSBattle were to center 2 divs with black background. The first div would have a top left border radius of 100% to create the circle arch. The second div would have a class that rotates it 180deg. Repeat the same inside the existing div but with a width/height that is half of the outer divs and yellow background.
- <img width="1717" alt="Screenshot 2024-09-19 at 1 23 03 PM" src="https://github.com/user-attachments/assets/a0860ea5-96b7-4168-9017-74ee3adc576f">

---

### Day 6: September 20, 2024 - Friday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Signed up for Women In Tech event <br>
✅ 100devs huddle


#### Thoughts

- Today's CSSBattle only took me ~3 min to get 100% match and one of my higher scores!!! The first time I did one it took me over an hour and I had to settle for 98% match 😭 Either I'm getting quicker or they're getting easier. Also remembered <body> tag is implicitly present in every html document so it's not necessary to add (especially since I'm trying to use the least amount of characters here) but obviously good practice to ensure proper structure and readability.
-  <img width="1719" alt="Screenshot 2024-09-20 at 1 28 00 PM" src="https://github.com/user-attachments/assets/dd290a46-981a-470b-96cc-69b97ca3c97f">
- Codewars problem was a cute one. I used the modular operator to determine which phrase corresponds to the last petal. My logic was for n and nx7 "i love you". for n and n+6 "a little", for n and n+5 "a lot" etc. or using the remainder of n*i. Since the phrases repeat every 6 petals, I can map the remainder of n % 6 to the appropriate phrase.
```
function howMuchILoveYou(petals) {
  const phrases = [
    "I love you",
    "a little",
    "a lot",
    "passionately",
    "madly",
    "not at all"
  ];
  
  return phrases[(petals-1) % 6]
}
```
- WOW ASTRO RELEASED ECOMMERCE STOREFRONT - https://github.com/withastro/storefront/
- THIS IS INCREDIBLE, I am saving to fork and play around with later

- Also, just found out theres an annual SheTo summit for women in tech looking to advance their career in leadership. I love this. I am manifesting that I will attend 2025. - https://www.sheto.org/summit
- Signed up for this event.  - https://women-in-tech.thisdotmedia.com/ 


---

<!---

### Day 1: September 9, 2024 - Monday

#### Todays's Progress

✅ 

#### Thoughts

- 

---

--->
