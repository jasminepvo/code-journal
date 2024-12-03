### Day 1: September 9, 2024 - Monday

#### Todays's Progress

✅ Completed 2 codewars problem <br>
✅ CSSBattle <br>
✅ UI for 75Hard Tracker

#### Thoughts

- Here we go again. Truth is, I prioritized my job over lifetime learning and consistency. As a new developer who just landed my first job in tech, which has been a dream of mine, I felt as if I owed my full time commitment and duty to performing as best as possible in my new role, since I was also making the most I've ever made in my life. Since then, I've learned tremendously and made an impact in that position which led me to fulfill even bigger dreams. I became a cofounder and frontend engineering lead, working with the most amazing programmer / friend currently who's doing big things at Google. I learned so much when it came to AI, backend, cloud, project mangement, marketing and all other responsiblities that come with a startup. I don't regret anything. Just looking forward to getting back to consistently coding/learning/growing each day regardless of where I end up next!
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
- <img width="1719" alt="Screenshot 2024-09-20 at 1 28 00 PM" src="https://github.com/user-attachments/assets/dd290a46-981a-470b-96cc-69b97ca3c97f">
- Codewars problem was a cute one. I used the modular operator to determine which phrase corresponds to the last petal. My logic was for n and nx7 "i love you". for n and n+6 "a little", for n and n+5 "a lot" etc. or using the remainder of n\*i. Since the phrases repeat every 6 petals, I can map the remainder of n % 6 to the appropriate phrase.

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
- Signed up for this event. - https://women-in-tech.thisdotmedia.com/

---

### Day 7: September 21, 2024 - Saturday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Signed up for Women Tech career fair <br>
✅ Started Total Typescript

#### Thoughts

- Today's CSSBattle was tricky. I knew it was a checkerboard pattern so I started off with the method to make nth elements have the transparent background but it is tedious.
- <img width="1717" alt="Screenshot 2024-09-21 at 4 06 50 PM" src="https://github.com/user-attachments/assets/cbc90878-e4ab-469a-947b-85ddcd8f55a6">
- Hmm attempted to use `repeating-linear-gradient` after seeing [this](https://www.30secondsofcode.org/css/s/10-css-background-patterns/) but it ended up being worse lol
- <img width="1715" alt="Screenshot 2024-09-21 at 4 42 46 PM" src="https://github.com/user-attachments/assets/c77c7290-8ac9-47f7-b8f2-5eed0692ee53">

- Codewars was easy today.

```
function reverseList(list) {
  return list.reverse();
}
```

---

### Day 8: September 23, 2024 - Monday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Total Typescript

#### Thoughts

- Today's CSSBattle was pretty easy, division sign haha. 2 circles and a rectangle. I probably could get more points if I used the `-webkit-box-reflect` across the x axis
- <img width="1715" alt="Screenshot 2024-09-23 at 1 51 55 PM" src="https://github.com/user-attachments/assets/4582be40-1a99-4747-8669-9840b0530d62">
- Codewars was a simple math equation, with the challenge to write it in one line of code. Here is what I submitted:

```
const findDifference = (a, b) => Math.abs((a[0]*a[1]*a[2])-(b[0]*b[1]*b[2]));
```

- I found these other solutions to be clever as well

```
function find_difference([a,b,c], [d,e,f]) {
  return Math.abs(a*b*c-d*e*f)
}
```

```
function find_difference(a, b) {
  return Math.abs(a.reduce((previous, current) => previous * current) - b.reduce((previous, current) => previous * current));
}
```

- Beginner's TypeScript: Lesson 1 - The Implicit "Any" Type error

  - Typescript requires you to assign a "type" to your parameters. If it's a number, string, boolean etc. This makes sense and I see the extra layer of readability and protection it serves.

  ```
  export const addTwoNumbers = (a: number, b: number) => {
    return a + b;
  };
  ```

  - When strict mode is enabled, you'll get the implicitly has 'any' type error whenever you leave type annotations out.

- Beginner's TypeScript: Lesson 2 - Working with Object Params

  - Here, the params is an object so we must assign each key a type

  ```
  export const addTwoNumbers = (params: { first: number; second: number }) => {
    return params.first + params.second;
  };
  ```

  - Another solution, use named alias type

  ```
  type AddTwoNumbersArgs = {
    first: number;
    second: number;
  };

  export const addTwoNumbers = (params: AddTwoNumbersArgs) => {
    return params.first + params.second;
  };
  - The other way is to use interface, however preferred method is the named alias type due to type can repesent anything (string, number, or boolean) AND less verbose error message

  ```

- Beginner's TypeScript: Lesson 3 - Set Properties as Optional
  - Adding a ? before the colon tells TypeScript that the property isn't required in order for the function to work.
  - `export const getName = (params: { first: string; last?: string }) => {`
- Beginner's TypeScript: Lesson 4 - Optional Parameters
  - Caveats: You can't put the optional argument before the required one.
- Beginner's TypeScript: Lesson 5 - Assigning Types to Variables
  - By adding : User to defaultUser, we're telling TypeScript that we want it to conform to our User interface.
  - `const defaultUser: User = {}`
  - `let a: number = 1`
  - useful for making sure variables match a certain type

### Day 9: September 24, 2024 - Tuesday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Total Typescript

#### Thoughts

- Today's CSSBattle was interesting. It says 100% match but I can clearly see the faint line of yellow for the difference. I probably could get more points if I used the `-webkit-box-reflect` across the x axis / less char.
- <img width="1282" alt="Screenshot 2024-09-24 at 3 18 08 PM" src="https://github.com/user-attachments/assets/845ab9cb-4fa9-4d0a-93a1-e73da10fc6dc">

- Today's Codewars was a practical use of objects

```
function greet(language) {
	// Use an object to map languages to greetings
  const greetings = {
    english: "Welcome",
    czech: "Vitejte",
    danish: "Velkomst",
    dutch: "Welkom",
    estonian: "Tere tulemast",
    finnish: "Tervetuloa",
    flemish: "Welgekomen",
    french: "Bienvenue",
    german: "Willkommen",
    irish: "Failte",
    italian: "Benvenuto",
    latvian: "Gaidits",
    lithuanian: "Laukiamas",
    polish: "Witamy",
    spanish: "Bienvenido",
    swedish: "Valkommen",
    welsh: "Croeso"
  };

  // Return the greeting if found, otherwise return "Welcome" as the default
  return greetings[language] || "Welcome";
  }
```

- Beginner's TypeScript: Lesson 6 - Constraining Value Types
  - This is a union type
  ```
  role: "admin" | "user" | "super-admin";
  ```
  - Anything can be added to a union type. For example, we can make a new SuperAdmin type and add it to the role:

```
 type SuperAdmin = 'super-admin'

 interface User {
   // ...other stuff
   role: "admin" | "user" | SuperAdmin;
 }
```

- Beginner's TypeScript: Lesson 7 - Working With Arrays

  - First syntax is to add square brackets, which I am more familiar with

  ```
  interface User {
    id: number;
    firstName: string;
    lastName: string;
    role: "admin" | "user" | "super-admin";
    posts: Post[];           //add square brackets
  }

  interface Post {
    id: number;
    title: string;
  }

  export const defaultUser: User = {
    id: 1,
    firstName: "Jasmine",
    lastName: "Vo",
    role: "admin",
    posts: [
      {
        id: 1,
        title: "How I eat so much meat",
      },
      {
        id: 2,
        title: "Why I don't eat more vegetables",
      },
    ],
  };

  ```

  - Second syntax is to use a generic type

  ```
  posts: Array<Post>
  ```

  - Both resolve into exactly the same thing. He mentions teaching generic type because the syntax is similar to promises, especially with maps, sets, records, things like that. But prefers the bracket syntax. Which I do too.

- Beginner's TypeScript: Lesson 8 - Function Return Type Annotations

  - Problem: how do we annotate the makeUser function to make sure it always returns a User?
  - Solution: define a User type and make sure the makeUser function explicitly returns an object of that type.

  ```
  import { expect, it } from 'vitest';

  interface User {
    id: number;
    firstName: string;
    lastName: string;
    role: 'admin' | 'user' | 'super-admin';
    posts: Post[];
  }

  interface Post {
    id: number;
    title: string;
  }

  /**
   * How do we ensure that makeUser ALWAYS
   * returns a user?
   */
  const makeUser = (): User => {
    return {
      id: 1,
      firstName: 'Jasmine',
      lastName: 'Vo',
      role: 'admin',
      posts: [
        {
          id: 1,
          title: 'Title 1',
        },
      ],
    };
  };

  it('Should return a valid user', () => {
    const user = makeUser();

    expect(user.id).toBeTypeOf('number');
    expect(user.firstName).toBeTypeOf('string');
    expect(user.lastName).toBeTypeOf('string');
    expect(user.role).to.be.oneOf(['super-admin', 'admin', 'user']);

    expect(user.posts[0].id).toBeTypeOf('number');
    expect(user.posts[0].title).toBeTypeOf('string');
  });
  ```

- Beginner's TypeScript: Lesson 9 - Typing Promises and Async Requests

  - This is the syntax for promises that will fix the Typescript error
  - `export const fetchLukeSkywalker = async (): Promise<LukeSkywalker> => {`
  - But this is the more common syntax, using type cast where data represents any since we don't know what will be returned

  ```
  export const fetchLukeSkywalker = async () => {
  const data = await fetch("<https://swapi.dev/api/people/1>").then((res) => {
    return res.json();
  });

  // cast the data to LukeSkywalker
    return data as LukeSkywalker;
  };
  ```

- Honestly not sure how I feel about this tutorial by TotalTypescript. It feels a bit backwards to me and although I am understanding since I've worked with Typescript a bit before, I don't feel like a true beginner would absorb this knowledge in a way that would help them gain a deep understanding. Just my personal opinion.

---

### Day 10: September 25, 2024 - Wednesday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Total Typescript

#### Thoughts

- Today's CSSBattle was the opposite. It says 99.6% match but I can't see the difference 🤔
- <img width="1262" alt="Screenshot 2024-09-25 at 6 03 41 PM" src="https://github.com/user-attachments/assets/2748aeeb-7b57-4650-9cf6-64f163ead240">

- Today's Codewars was awesome, I love that my solution was top best practices / clever today! Very practical use too

```
psuedocode:
// search the array of strings and store the string first in alphabetic order
// loop through the string and add *** between each of its letters, return this
solution:
const twoSort = (s) => s.sort()[0].split('').join('***');
```

### Day 11: September 26, 2024 - Thursday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Coffee Chat with Yana Zaynullina <br>
✅ Work on portfolio

#### Thoughts

- Today's CSSBattle was sooo frustrating. I couldn't get the half circle to match! This is definitely the worst I've done
- <img width="861" alt="Screenshot 2024-09-26 at 11 48 01 AM" src="https://github.com/user-attachments/assets/604b6de2-cf5d-43cd-9ea3-d06232a799d5">
- Attempted again, this time adding a window for the half circle with overflow hidden. Still only 99.9%
  <img width="1402" alt="Screenshot 2024-09-26 at 3 12 14 PM" src="https://github.com/user-attachments/assets/65ae3dfc-613c-44fd-ae16-2a033159a98c">

- Today's Codewars was simple, I definitely had to refactor after

```
function peopleWithAgeDrink(age) {
    if (age<14)
      return "drink toddy";
    else if (age>=14 & old<18)
      return "drink coke";
    else if (age>=18 & old<21)
      return "drink beer";
    else
      return "drink whisky";
};
```

```
const peopleWithAgeDrink = (age) =>
  age < 14 ? "drink toddy" :
  age < 18 ? "drink coke" :
  age < 21 ? "drink beer" : "drink whisky"
```

- Watched Ellie's portfolio roast and that definitely inspired / reminded me to work on my portfolio again. So today I finished my hub. The masonry layout is ready to take content from Storyblok CMS which was cool and easy to implement with Astro. Also typed up a blog draft on the portfolio layout design.

---

### Day 12: September 27, 2024 - Friday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>

#### Thoughts

- Today's CSS Battle was just overlapping squares with borders and backgrounds
- <img width="1390" alt="Screenshot 2024-09-27 at 8 14 38 PM" src="https://github.com/user-attachments/assets/01d8d496-2d7a-4dbe-88df-c8b597e30c55">
- Codewars today

```
function findMultiples(integer, limit) {
  let multiples = [];

  for (let i = integer; i <= limit; i += integer) {
    multiples.push(i);
  }

  return multiples;
}
```

---

### Day 13: September 28, 2024 - Saturday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Worked on my portfolio projects page <br>

#### Thoughts

- I was able to get a pretty dry solution today! I used replace() method to replace all characters in a string with an empty string. The characters I replaced were vowels so I used regex character set to match all the vowels followed by the g which means global to match all instances of the char even if there is a repeat.
  ` const shortcut = (string) => string.replace(/[aeiou]/g, '')`

---

### Day 14: September 29, 2024 - Sunday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Worked on my portfolio projects page <br>

#### Thoughts

- Thought process was to use a ternary operator since xor represents true as long as a and b are not the same
  `const xor = (a, b) => a !== b ? true : false;`

---

### Day 15: September 30, 2024 - Monday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Worked on my portfolio projects page <br>

#### Thoughts

- Today's CSSBattle I learned how to create a triangle with CSS! Pretty cool stuff. Since I needed a right triangle with the diagonal running from the bottom left to top right, the trick was to make the border left contains the whiteish color, while the border bottom contains the yellow color. I estimated the margin would be 40px, so 200px - (40px\*2 sides) = 120px to set the border width.
<img width="1539" alt="Screenshot 2024-09-30 at 4 07 51 PM" src="https://github.com/user-attachments/assets/bc966704-5275-4b1a-8658-d459073e5b3f">

- Todays Codewars was weird, I didn't realize American floor systems were like this? All the apartments I've been in have been normal where first floor is the first floor and so forth. Anyway this is how I solved it and made the most sense to me. The dry solutions are a bit hard to read for this one imo!

```
function getRealFloor(n) {
  if (n <=0) return n;
  if (n >=13) return n-2;
  return n-1;
}
```

---

### Day 16: October 1, 2024 - Tuesday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Registered for Hacktoberfest <br>
✅ Worked on portfolio <br>
✅ Coffee chat with Marilyn

#### Thoughts

- CSSBattle definitely took me some time to figure out. I learned how to break the circle up into quarters using border-color transparency, then using a radius to create the hollowed circled / arch
```
    border-radius: 50%;
    width: 240px;
    height: 240px;
    box-sizing: border-box;
    border-width: 60px;
    border-style: solid;
    border-color: #E25C57 transparent transparent transparent;
    transform: rotate(45deg);
```
- The part I struggled with getting pixel perfect was the positioning of the second circle arch. I thought I could just rotate it from the first positioning but that turned out trickier than expected
- Nevertheless this one was fun and I learned something new!
-  <img width="1527" alt="Screenshot 2024-10-01 at 3 28 50 PM" src="https://github.com/user-attachments/assets/92932e77-77c9-456a-a9c9-bdc38327c746">
- Codewars: originally would have approached this thinking to store the first name before the " " into an array, and push the last name into the array.. and then return last name first name as a string. But I knew there was a simpler and efficent way to approach this using string methods like reverse, split, join. Pretty cool these came back from muscle memory considering I haven't used them in awhile!
- Dry solution: `const nameShuffler = (str) => str.split(' ').reverse().join(' ');`
- I joined Hacktoberfest! Super excited to contribute to open source this month. 
- Also, finished my projects page on my portfolio! 
---

### Day 17: October 2, 2024 - Wednesday

#### Todays's Progress

✅ Coffee chat with mentee <br>
✅ Posted on LinkedIn <br>
✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ Worked on Hacktoberfest issue <br>
✅ Worked on portfolio <br>
✅ Huntober <br>

#### Thoughts

- Mentee call went well. She's made so much progress in a short week, also she was so excited this week to show off what she made which made me happy to see considering she said nothing excited her in the beginning! Went over time a bit but it's okay, we're both learning. Set an agenda for the next 2 meets!
- Codewars was a very easy if/else statement
- CSSBattle TIL how to create a polygon using clip path!!! Not perfect but I'm happy I learned something new :)
<img width="1515" alt="Screenshot 2024-10-02 at 1 56 14 PM" src="https://github.com/user-attachments/assets/813fcc6d-e1ed-4fe8-bdc4-68c05559dbe9">

- Hacktoberfest
  - Got assigned an issue from this OS project, I love working on UI - https://github.com/devhub-ai/devhub/issues/34
- Portfolio
  - Somehow I got disconnected from Github so I spent some time reconnecting.
  - Hmm some reason my ssh key was removed? I added a new ssh key and successfully reconnected yay, pushed my changes!
  - Updated my README.md, I love making these. Documentation is so fun to me 😅

---

### Day 18: October 3, 2024 - Thursday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>
✅ ViteConf <br>
✅ Worked on portfolio <br>
✅ ANKI <br>
✅ Huntober <br>

#### Thoughts

- DailyCSS Battle today was hard to match this perfect hollow oval shape, only got 99%
- But TIL how to make an oval, W3schools always saves my life - https://www.w3schools.com/howto/howto_css_shapes.asp
- <img width="1532" alt="Screenshot 2024-10-03 at 12 33 10 PM" src="https://github.com/user-attachments/assets/2c13ec89-c958-4368-b155-554530867a65">
- ViteConf was cool, lots of interesting talks. I'll be honest some made no sense to be because it was like hearing a foreign language, but very cool to see nonetheless. Vite has grown so popular now compared to when I first used it 2 years ago and fell in love with how fast, easy and amazing DX it was. I remember making a LinkedIn post about how everyone should stop using cra and soley use Vite. I LOVEEE that Astro uses Vite.
- <img width="1456" alt="Screenshot 2024-10-03 at 12 34 09 PM" src="https://github.com/user-attachments/assets/bf243b04-e56c-4e83-aa84-2ee0b5d98831">
- My favorite talk of the day.
  - Wow I love how easy whiteboard guy makes everything look. He created a document editor, search function and added AI (search w llm) all within 20 min
  - I need to look over the vector search logic again
  - https://github.com/bholmesdev/local-first-vite-conf-2024
  - You can put sql and ai in the browser
  - Learned about gemma :o  
- <img width="1475" alt="Screenshot 2024-10-03 at 2 51 47 PM" src="https://github.com/user-attachments/assets/e47204d3-f93f-4474-b58b-12c5c5555143">
- Portfolio is making progress...
  - Home/about page now has a hero w an image annd intro that took me way too long to write haha

---

### Day 19: October 4, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Recruiter call <br>
✅ Coffee Chat w Tony <br>
✅ Huntober <br>

#### Thoughts

- Call went so good! Catching up with Tony was amazing. Huntober was great as always. It's been a long day but fruitful day :)

---

### Day 20: October 9, 2024 - Wednesday

#### Todays's Progress

✅ Coderbyte <br>
✅ Portfolio - about page <br>
✅ ANKI <br>

#### Thoughts

- Took a few days off to spend with family visiting from out of town. It was a nice break! 
- Practiced a coderbyte problem, talking out loud as if it was a live whiteboard interview. This is the first time I've ever done this so def a new experience to get comfortable with. I felt it went well. Initially I blanked LOL but writing comments, re-reading everything, then writing the code and re-reading the code after really helped. Used P.R.E.P!
- I even deleted everything and wrote it again. But I am so mad at myself bc when I wrote it again, I had the wrong syntax and added a = when I shouldnt have so the code didnt run and I got a 0. Ahh live and you learn, now I will be extra extra cautious
```
import React, { useState } from 'react';
import { createRoot } from 'react-dom/client';

function Toggle() {
  // initialize the state, isOn will be true, setIsOn 
  // is the function used to udpate the state
  const [isOn, setIsOn] = useState(true);

  // create a function called handleClick that is going 
  // to use the setIsOn function that updates the state
  // to toggle from prevstate (false) to not prev state (true)
  function handleClick() = {
    setIsOn(prevState => !prevState);
  }
  
  // then we use the function to conditionally render the 
  // button text based on the state 
  // isOn ? "ON" : "OFF"
  // so if prev state of isOn = ON, then !prev state = OFF

  // attach an event listener onClick to the button which 
  // triggers the handleClick function when the button is clicked
  return (
    <button onClick={handleClick}>
      {isOn ? "ON" : "OFF"}
    </button>
  );
}

const container = document.getElementById('root');
const root = createRoot(container);
root.render(<Toggle />);
```

- Worked on my portfolio again. Setting a goal now to be done with it by Tuesday, October 15.
  - 10/10 hero main
  - 10/11 hero main
  - 10/12 tech stack, socials / where to find or contact me, glimpse of projects (shown as cards)
  - 10/13 blog
  - 10/14 blog

---

### Day 21: October 10, 2024 - Thursday

#### Todays's Progress

✅ Posted on LinkedIn <br>
✅ ANKI <br>
✅ Huntober <br>

#### Thoughts

- Good Huntober session on LinkedIn. Did some updates to my profile and posted! Posting has been a fear of mine so I'm overcoming it! I have always overthought "What should I post" or "What is appropriate?" - but I'm doing a new take on this. It's a platform with of all my professional connections, that doesn't mean it can't be fun or has to be shallow and surface level. I've been doing so much inner work on myself lately and finding my voice. I'm just going to be me from here on! 

---

### Day 22: October 11, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Huntober <br>
✅ Portfolio - about page <br>

#### Thoughts

- Pretty happy about where the cards are right now, definitely need to go back and update the content but everything else is good!
- Power hour for huntober was fire as usual. Listening to others be in a spot I was once in and hearing their emotions around it, definitely makes me feel empathetic for them. Hope the words of advice I gave we're helpful. 

---

### Day 23: October 12, 2024 - Saturday

#### Todays's Progress

✅ Portfolio - about page <br>

#### Thoughts

- Decided to switch directions with what I originally wanted in the main hero, but I'm getting somewhere with design...

---

### Day 24: October 13, 2024 - Sunday

#### Todays's Progress

✅ Portfolio - about page <br>

#### Thoughts

- SO HAPPY WITH THE DESIGN NOW. Finally got full clarity with what I want. Wrote it up in the blog!
- Mockup the main hero in Excalidraw

---

### Day 25: October 14, 2024 - Monday

#### Todays's Progress

✅ Portfolio - about page <br>

#### Thoughts

- New design definitely = more work on the layout since everything is free standing 😅 BUT I'm getting so good at grid. I love grid. I used to only use flex but grid is truly OP.
- Mockup the rest of the about page with the new design theme in Excalidraw. TBH I had no direction where I was going and I knew if I sat on Figma, it wouldn't go anywhere or would take 10x as long. As I developed, it allowed me to reframe what I truly wanted the user to see and experience, and reframe my design from boring to me :)
- I'm really truly loving how everything is coming together. 
<img width="630" alt="Screenshot 2024-10-15 at 1 41 19 PM" src="https://github.com/user-attachments/assets/56b54929-4c12-43ee-ab85-5e475de1d1e4">

---

### Day 26: October 15, 2024 - Tuesday

#### Todays's Progress

✅ Post on LinkedIn / X <br>
✅ Call w Engineering Manger <br>
✅ Mentee call - mock interview <br>
✅ Portfolio - projects <br>
✅ Huntober <br>
✅ DSA practice <br>


#### Thoughts

- Finally updated the community w my current situation open for new opportunities, received some recruiter interest so yay :)
- Call was ok, company sounds fantastic but I wish I had been more prepared going into it. It was with a friend and I made the horrible assumption it would be casual professional but it ended up being professional professional and I was a bit flusterered when speaking. I wasn't my typical confident self but we will see what happens. 
- My mentee Yana did so freaking well in the technical mock interview. We did the leetcode question over unique elements and she nailed it. Communicated throughout, asked questions and solved it efficiently with understandings of time and space. She is killing it. So excited for her interview, I know she will do so well. Moments like this make me so happy :)
- <img width="1865" alt="Screenshot 2024-10-15 at 3 45 57 PM" src="https://github.com/user-attachments/assets/0026ad32-d4a6-4b82-9b79-5cdaf33e1e92">
- Huntober was DSA practice which I am taking more seriously now bc I want to improve and also bc I have an upcoming interview. Leon went over Gauss trick and I started watching freecodecamp dsa algo w javascript - which started off with Stacks


---

### Day 27: October 16, 2024 - Wednesday

#### Todays's Progress

✅ Women Tech Network Job Fair & Summit 2024 <br>
✅ DSA practice with ChatGPT <br>

#### Thoughts

- Long long day of conference. So many good talks, talked to lots of recruiters and other women in tech and networked on LinkedIn.
- Notes here: https://docs.google.com/document/d/1S06DF7jTuDpF2t50k6es5VH_jvNNqIBKKjmO2o1c2GI/edit?usp=sharing
- So I started watching the youtube vid again on sets and queue but I was folding laundry at the time and it was difficulty for me to feel like I was fully grasping the concepts. I learn best by doing so I pulled out ChatGPT and used the voice feature to talk to the AI to review the dsa and have me repeat them back. Repetition helps a lot, especially verbal repeition and I would reply back in my own voice / examples. It ended up being super fun actually and AI even had quizzes for me to do which I also found fun. I used Gale? voice with a slight British accent which was very engaging to me and satisfying hearing her say "Yess you're right on the money" or "You've absolutely nailed it" in her accent.
- No coding, I am feeling a bit beat up so I'm going to rest up so I can hit up leetcode tmr and finish up my portfolio!

---

### Day 28: October 17, 2024 - Thursday

#### Todays's Progress

✅ Recruiter call <br>
✅ BANKI <br>
✅ Huntober <br>
✅ Leetcode <br>

#### Thoughts

- Getting a lot more recruiters messaging me right now so been responding to those. Turned down a React dev role at BOA for 40/hr but that is way below what I'm looking for and I'm proud for turning it down. I feel so blessed and proud of myself for having a savings for the first time in my life so I can stress less about money and not be desperate for the first thing. I know my worth and what I deserve and I love that.
- I am super excited for my interview next Wed so most of my time has been dedicated towards preparing for that. This will be the first whiteboarding technical interview I've ever had and I want to / will do well. Practicing dsa and did my first leetcode question today. My mindset has shifted a lot in the past year. I'm not longer saying the words "I can't do that", and reframing my mindset to "I can and I will bc there is nothing in this world I can not do if I put my mind to". <3 
- Doing BANKI is so great this time around bc I feel like I have so much to talk about that I don't know where to begin or which to talk about, which is a great problem to have. I have gained so much experience in a short time and I'm so proud of myself!!!! :)
- Huntober was great, I'm finally grasping Big O notation
- Time is the number of operations you do
- Space is how much memory is being used
- O(n) is generally the most efficient
- I used to struggle so hard with learning dsa but I realize it wasn't me, it was the way it was taught.
- The Leetcode question I did was the two sum question. I learned hash map.
  - initialize a new empty map
  - loop through the length of the array
  - initialize complement variable that serves as the target - arr index, (target:9, i:2 = complement is 7)
  - check the map to see if the complement exists in the map
  - if it exist, return the complement and the index in the array
  - otherwise set the current num and its index in the map
  - return empty arr if no solution is found

---

### Day 29: October 18, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ React Inteview Q's <br>

#### Thoughts

- Deep diving into React state management and hooks again for the interview since it will be building a component (depth in specialization)

---

### Day 30: October 21, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Coffee Chat w Richard <br>
✅ Study React <br>
✅ Huntober <br>

#### Thoughts

- Spent most of the day reviewing React concepts and practicing state management with the counter component
- https://codesandbox.io/p/sandbox/loving-mclean-5gs52s
  
---

### Day 31: October 22, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Coffee Chat w Deja <br>
✅ Mock Interview w Krista <br>
✅ Huntober <br>

#### Thoughts

- Reviewed React concepts again, useEffect and loading/data/error state management
- https://codesandbox.io/p/sandbox/vkygtt 

---

### Day 32: October 23, 2024 - Wednesday

#### Todays's Progress

✅ Interview <br>
✅ Huntober <br>

#### Thoughts

- Honestly was super nervous. There were no behavioral questions asked. These were the questions:
  - What experience do you have with testing?
  - How do you do unit test what are you testing for?
  - How do you render a component?
  - What are you looking for when you render a component?
  - What do you do when you get a design, what is your process?

- React coding assessment: Implement a C-shaped grid that behaves this way
  - Square toggles between white / green
  - If all squares are toggled green, automatically toggle white in the reverse order they were toggled green
 
- At the end of the day, the interview went the way it should have. For my first live coding interview, I'm pretty proud of myself. I blanked on simple things but the feedback I got was I communicated well so I'll take it. It definitely taught me areas I still need to strengthen!
- It also gave me an understanding of the company a bit more and I realized it wasn't for me. As it should be, the hiring process goes both ways. It's important to me to make sure I'll be happy there bc I'll be dedicating part of my life to it. I'm proud of myself for having this mindset now, much different to where I was 2 years ago.
- Took the rest of the day to debrief

---

### Day 33: October 24, 2024 - Thursday

#### Todays's Progress

✅ Mentee call <br>
✅ Recruiter call <br>
✅ Huntober <br>

#### Thoughts

- Love meeting with my mentee, she shared her first live coding interview experience and it made me happy that the mock interview we did really helped her.
<img width="843" alt="Screenshot 2024-10-24 at 12 38 57 PM" src="https://github.com/user-attachments/assets/a7d91387-c41a-47c5-b0e0-0d0ccb6b2607">

- Recruiter call went AMAZING. I was honestly feeling beat down by the interview yesterday but talking to the recruiter gave me life again. This time, I could feel it in my heart, gut and soul that I REALLY want this opportunity. It aligns perfectly with me in terms of being able to make an impact, the culture, startup environment w financial stability, structure within the engineering team, products that I'd be working on would be exciting and geared towards small businesses which I'm passionating about helping coming from a family with a small business <3

---

### Day 34: October 25, 2024 - Friday

#### Todays's Progress

✅ Build new project <br>
✅ Huntober <br>

#### Thoughts

- The interview question made me really want to go back and solve it because I know it's something I could. Nothing is out of my reach or scope of knowledge. It is the first time I've come across that situation and I just needed time to solve it is all so I did. I also wanted to share the component with others / keep it in memory for myself to review which led to me building a React component library. I'm just going to dump components that I build over time into here - https://react-jasminepvo.netlify.app/
- I will eventually also go back and rebuild components that I've built over the years. Just a fun little coding day to destress :)

---

### Day 35: October 28, 2024 - Monday

#### Todays's Progress

✅ Come up with new study guide
✅ Practice Leetcode #139 

#### Thoughts

- Word Break really threw me for a loop. It was wayyyy harder than I thought and took me forever. Quite literally forever. But I'm happy I took the time to go through and actually understand it, also helped me get a better understanding of time/space complexity.
- Made me think of real world examples it would be used in which was cool:
  - Spell Checking and Word Segmentation in Search Engines
  - Text Autocomplete and Predictive Text
  - Decoding Languages Without Spaces (e.g., Chinese, Japanese)
  - Password cracking
- Did more research on the company and used ChatGPT to help me come up with a study guide while I prep for this next interview, focusing on my weakness of DSA / leetcode

---

### Day 36: October 29, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 5 Leetcode problems <br>
✅ Huntober <br>

#### Thoughts

- Watched Neetcode yt vid to refresh on the top data structures (arrays, linked list, hash map, queue, binary tree, trie, heap, graphs)
- - Started https://leetcode.com/studyplan/30-days-of-javascript/
  - Solved all the closures (level easy) #2667, #2620, #2704, #2665
  - ++count (pre-increment operator will count first then return the new, incremented value)
  - count++ (post-increment operator will increment but return the original value before the increment
  - syntax for creating methods inside a function
    ```
    const expect = (val) => {
    return {
        toBe: (otherVal) => (val === otherVal) ? true : ( () => { throw new Error("Not Equal"); })(), 
        notToBe: (otherVal) => (val !== otherVal) ? true : ( () => { throw new Error("Equal"); })()
       }
    };
    ```
- huntober went over hash maps
```
function maxCharacter(str) {
  //map + count + maxChar
  let charMap = {},
      count = 0,
      maxChar = null
  //map for chars in str + freq
  for(const char of str) {
    // if charMap[char] exists (if there is a key of that letter and it is therefore truthy) then increment it by one. else set it to one (if it is falsy)
    charMap[char] = charMap[char] + 1 || 1
  }
  //loop and find most freq char
  for(const char in charMap) {
    if(charMap[char] > count) {
      count = charMap[char]
      maxChar = char
    }
  }

  return maxChar
}
console.log(maxCharacter('Hello World!'), 'l')

//Time: O(n)
//Space: O(n)
```
For anyone who is confused, these two code snippets do the same thing:
```
if (charMap[char] == null) {
  charMap[char] = 1;
}
else {
  charMap[char] += 1;
}
```
```
charMap[char] = charMap[char] + 1 || 1
```
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Property_accessors
- https://www.freecodecamp.org/news/short-circuiting-in-javascript/

- That was A LOT. Spent the night playing top golf with friends to debrief and wind down letting my brain soak in everything

---

### Day 37: October 30, 2024 - Wednesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problem <br>
✅ Huntober <br>

#### Thoughts

- Super locked in. Spent the day going over the basic data structures and when you'd use them. Attempted task scheduler but had to look it up
- huntober went over more hash maps

---

### Day 38: October 31, 2024 - Thursday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 3 Leetcode problems <br>
✅ Huntober <br>

#### Thoughts

- Went over task scheduler again, cleaning up my notes and reviewing for repetition
- Solved easy array problems, mainly practicing PREP
- huntober went over a problem i recognized, lets goo! I knew exactly how to solve it, the most efficient way and how to talk through it :)

---

### Day 39: October 30, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>
✅ Huntober <br>

#### Thoughts

- Continued on solving easy arrays and recgonizing the patterns
- Planned out my interview schedule w GG
- Scheduled an interview for next week
- Watched system design mock interviews over Spotify and Tik Tok

---

### Day 40: Nov 4, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 1 Leetcode problem <br>
✅ Huntober <br>

#### Thoughts

- We are trucking along the dsa train and I'm actually starting to enjoy it. I can recognize the patterns more as I keep exposing myself to it. I remember when I would open Leetcode, stare at it for 10 min and close it. It's just a skill like working out and with continuous repetition and progressive overload, I can master it. There is quite literally nothing I can't do!
- Reviewed task scheduler AGAIN and this time it went by a lot quicker. I could visualize the iterations this time. Still messed up syntax trying to solve though but it's okay
- Huntober was fun, I really like hash maps. we went over two sum which I have solved already so I recognized it but Leon solved it a different way than I initially did so that was cool to see.

---

### Day 41: November 5, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 1 Codewars 6kyu <br>
✅ Practice 1 GreatFrontend problem <br>
✅ Practice 2 Leetcode <br>
✅ Huntober <br>

#### Thoughts

- Anki review went well. 80 cards in 22.44min today
- Started the HackerRank 1 month preperation kit. Solved plus minus. This seemed difficult initially bc of all the math in the description but it was pretty simple after walking through the PREP method. The only thing I had to look up was how to place the decimal at a fixed spot though using `.toFixed(6)`
- I am using both Leetcode and HackerRank bc that's what the recruiter said to study
- Read up on system design concepts and added to anki, also read through the interview process
- Mock interview on CoderPad to simulate real time coding with the IDE I will be using, and practiced communication (did a react todo problem)
- My initial approach with this Codewars 6kyu. Passed with Time: 824ms
- <img width="1315" alt="Screenshot 2024-11-05 at 2 10 43 PM" src="https://github.com/user-attachments/assets/d405d523-825f-4cd6-959b-2f396689775b">
- Here is the appraoch from ChatGPT. Passed with Time: 819ms
- <img width="1511" alt="Screenshot 2024-11-05 at 2 14 21 PM" src="https://github.com/user-attachments/assets/51cf2a80-ac18-4634-8ba8-26e3c783a505">
- Only a 5 millisecond difference. So I'm assuming either would work. 

- Neat way to return thirty minute intervals 
```
function getThirtyMinuteIntervals() {
    const intervals = [];
    const totalMinutesInDay = 24 * 60; // 24 hours * 60 minutes = 1440 minutes

    for (let minutes = 0; minutes <= totalMinutesInDay; minutes += 30) {
        const hours = Math.floor(minutes / 60).toString().padStart(2, '0');
        const mins = (minutes % 60).toString().padStart(2, '0');
        intervals.push(`${hours}:${mins}`);
    }

    return intervals;
}

// Usage
console.log(getThirtyMinuteIntervals());
[
    "00:00", "00:30", "01:00", "01:30", "02:00", "02:30", "03:00", "03:30",
    "04:00", "04:30", "05:00", "05:30", "06:00", "06:30", "07:00", "07:30",
    "08:00", "08:30", "09:00", "09:30", "10:00", "10:30", "11:00", "11:30",
    "12:00", "12:30", "13:00", "13:30", "14:00", "14:30", "15:00", "15:30",
    "16:00", "16:30", "17:00", "17:30", "18:00", "18:30", "19:00", "19:30",
    "20:00", "20:30", "21:00", "21:30", "22:00", "22:30", "23:00", "23:30",
    "24:00"
]
```
- Solved another hash map problem, this was actually fun - https://leetcode.com/problems/first-letter-to-appear-twice/description/
- Added algorithm pattern / leetcode templates to anki
- huntober cancelled bc election day
- Another fun leetcode: https://leetcode.com/problems/check-if-the-sentence-is-pangram/submissions/1444295301/

---

### Day 42: November 6, 2024 - Wednesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>
✅ Recruiter call with Leap Metrics <br>
✅ Huntober <br>

#### Thoughts

- Recruiter call went well! I thought it was going to be a screening but it actually turned into a behavioral interview. Nevertheless, I passed and am moving forward. 
- Added a ton more system design concepts to ANKI
- Huntober was power hour, good energy
- Worked on leetcode group anagrams - https://leetcode.com/problems/group-anagrams/description/
- Read up on coding patterns

---

### Day 43: November 7, 2024 - Thursday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>
✅ Huntober <br>
✅ Dallas Software Developers meetup <br>

#### Thoughts

- Marcia gave the great idea to put leetcode problems into ANKI so I started doing that!
- Working on 2 pointers now - roman to integer, valid palindrome
- Huntober was great, went over fibonacci 
- It was great seeing everyone again at the meetup and catching up with Danny and Noel :)
- Met new faces - Morat, Jordan  

---

### Day 44: November 8, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>
✅ Huntober <br>

#### Thoughts

- LeetCode with Maye, we did closest number to zero
- I reviewed Two Sum again
- Found Leetcode coding patterns and starting to recognize them!
- Huntober was fibonacci again, second to last session :( 

---

### Day 45: November 9, 2024 - Saturday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- LeetCode with Maye - worked on #268 missing number
- It was cool to see the different ways to solve it:
- using a simple for loop
- map
```
const n = nums.length;
    const map = new Map();
    
    // Store each number in the map
    for (let num of nums) {
        map.set(num, true);
    }

    // Check for the missing number in the range [0, n]
    for (let i = 0; i <= n; i++) {
        if (!map.has(i)) {
            return i; // Return the missing number
        }
    }
```
- approaching it from a sum/difference perspective
```
var missingNumber = function(nums) {
    const n = nums.length;
    // Calculate the expected sum of numbers from 0 to n
    const expectedSum = (n * (n + 1)) / 2;
    // Calculate the actual sum of elements in the array
    const actualSum = nums.reduce((acc, num) => acc + num, 0);
    // The missing number is the difference
    return expectedSum - actualSum;
};
```
- Reviewed system design

---

### Day 46: November 10, 2024 - Sunday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- Reviewed system design and ANKI
- No leetcode today
- Spent time helping my mom, eating her pho, getting the christmas tree and buying a new ball for Coda

---

### Day 47: November 11, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- Leetcode with Maye: merge strings alternatively, max water container
- both two pointers again
- Put up the christmas tree at night, she's so cute!

---

### Day 48: November 12, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- Leetcode with Maye: Intervals problem - [meeting schedules ii](https://neetcode.io/problems/meeting-schedule-ii)
- Man that problem took us awhile but I have a great understanding on it now. We went over the different approaches using two pointers and greedy algorithm. I liked both but two pointers makes the most sense to me. Both are O(nlogn) time and O(n) space too!
- Also practiced speed typing. Made me chuckle
<img width="1095" alt="Screenshot 2024-11-14 at 11 55 56 AM" src="https://github.com/user-attachments/assets/4f022e35-35a9-4602-8248-ee8eeb43576c">

---

### Day 49: November 13, 2024 - Wednesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- No Leetcode with Maye
- Went over sliding window pattern

---

### Day 50: November 14, 2024 - Thursday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- Leetcode with Maye: meeting rooms
- went back over merge strings alternatively

---

### Day 51: November 15, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>


#### Thoughts

- Leetcode with Maye: nonoverlapping intervals
- best time to buy and sell stock

---

### Day 52: November 16, 2024 - Saturday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- Leetcode with Maye: nonoverlapping intervals

---

### Day 53: November 17, 2024 - Sunday

#### Todays's Progress

✅ ANKI <br>
✅ Practice 2 Leetcode problems <br>

#### Thoughts

- insert interval and valid parenthesis

---

### Day 54: November 18, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Practice Leetcode <br>

#### Thoughts

- Leetcode with Maye: insert interval

---

### Day 55: November 19, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice Leetcode <br>

#### Thoughts

- Leetcode with Maye: mock interview over group anagrams

---

### Day 56: November 20, 2024 - Wednesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice Leetcode <br>

#### Thoughts

- Leetcode with Maye: mock interview over merge intervals

---

### Day 57: November 21, 2024 - Thursday

#### Todays's Progress

✅ INTERVIEW DAY <br>

#### Thoughts

- WOW I KILLED IT! The interview ended up being very fun. It was related to intervals which is what I've been studying!!! My interviewer was very cool, loved my approach. Solved for the first day of the week but then the second day of the week was giving the wrong output which we were both trying to debug for 5 min. He had to end it bc we went 15 min over time haha! We were both very into it and it really did feel fun. I realized later it was due to having only ">" instead of ">=" 😆
- Went out for lunch after to celebrate all the hard work and got an email less than an hour later notifiying me that I'm moving forward to the next round!!!
- Luck is preparation meetings opportunity :) 

---

### Day 58: November 22, 2024 - Friday

#### Todays's Progress

✅ ANKI <br>
✅ Leetcode with Maye <br>
✅ Mentee call <br>
✅ 100Devs Huddle <br>

#### Thoughts

- Spent time going over my interview with Maye
- Caught up with my mentee, happy to hear from her and catch up
- 100devs huddle was a good power hour

---

### Day 59: November 23, 2024 - Saturday

#### Todays's Progress

✅ ANKI <br>

#### Thoughts

- Honestly crashed after the interview and all the explaining the day after. Took today to chill and take it easy. Had friendsgiving dinner to cook for!
- https://www.youtube.com/watch?v=i53Gi_K3o7I&t=199s

---

### Day 60: November 24, 2024 - Sunday

#### Todays's Progress

✅ ANKI <br>
✅ System Design <br>

#### Thoughts

- Watched some youtube videos on system design and going over the resources given
- https://interviewing.io/guides/system-design-interview

---

### Day 61: November 25, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Leetcode with Maye <br>
✅ System Design <br>

#### Thoughts

- Leetcode: easy - return # of unique Element that exists once
- Looked over more interviews. Scheduled availability for upcoming interviews
- Practiced on FigJam
- https://github.com/donnemartin/system-design-primer

---

### Day 62: November 26, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅ Practice System Design <br>

#### Thoughts

- Mock interview with Maye: ahhh I didn't do great. I got through the radio framework but not efficiently and didn't realize most of the time should be spent on optimization. Definitely need to improve on this area 
- Requirements - 9 min
- Architecture / High Level Overview - 12 min
- Data Model - 6 min
- Interfacees - 12 min
- Optimization - 24 min
- https://www.greatfrontend.com/system-design/framework
- https://www.youtube.com/watch?v=5vyKhm2NTfw

---

### Day 63: November 27, 2024 - Wednesday

#### Todays's Progress

✅ Mock Interview <br>
✅ Mentee Call <br>
✅ Mock Interview <br>
✅ Recruiter Prep <br>

#### Thoughts

- Ngl, I am feeling OVERWHELMED! AH! I know I need to just breathe, study, practice and repeat. System designs is kicking my butt. I designed the frontend architecture for FR but when it comes to timeboxing everything in 60 min + data model + api AND talking about optimization.. that's where it starts to stress me out. My mock interviewer gave me great advice to record myself and listen to gaps of silence etc to be as efficient as possible. Just going to take reps, like building muscle. I GOT THIS though! I am capable of anything and this being so hard of a challenge will only make the offer more rewarding :)
- ALSO my recruiter is amazing. She took 45 minutes out of her day to prep me for these interviews with so much detail so there is no way I'm going to let her (or my referral) down.

---

### Day 64: November 28, 2024 - Thursday

#### Todays's Progress

✅ ANKI <br>
✅ System Design Prep <br>

#### Thoughts

- FCC Crash course was good for a high level overview and better understanding of best API practices, learning more about performance. Also thinking through frameworks and my decision behind them. Always make sure I explain what to design and why. Wrote all the notes in my iPad!
- https://interviewing.io/guides/system-design-interview Tips
  - Always question the parameters of the service - what type of users does it serve, what type of traffic can it expect, what limits will it have?
  - Mid level roles expect you to take moments of pause, let the interviewer guide
  - Sr level roles expect you not to have silence, you should be leading the interview
  - Don’t say things because you think you’re supposed to say them. This often occurs when candidates name specific brands of technologies (e.g., “Kafka” or “Cassandra”). I’m going to use a NoSQL db because of [insert brief rationale].
  - Make decisions. DO SAY THIS - "We could use this type of DB, or this other, or that other, and these are some pros and cons… And based on all these tradeoffs, I’ll use THAT type of DB."
  - Whatever decision you make, explain why. In a system design interview, why is more important than what. For anything you say, be prepared to explain why.
  - "I don't know, I'm definitely going to look that up right after this interview, but if I had to give my best guess I'd say... [x] and here is why [explanation/thought process]
  - <img width="972" alt="Screenshot 2024-11-28 at 9 44 55 PM" src="https://github.com/user-attachments/assets/44fd2715-1bbd-4086-99c7-46163d698db8">
  - Acknowledge and affirm your interviewer. Start with “sure,” “OK,” or “yes,” so they are open to what you’re saying. This results in them being less likely to push back against your pushback.
  - The best language to demonstrate collaboration is “We” or “Let’s.” For example: “We could take out the cache. However, if we did that one drawback would be [insert technical reasoning here]…”
  - When we say “handwave stuff,” this means that you can say, “I’m going to skip going into [detailed thing] for now, but if we want, we can come back to it later.”
  - Be conscious of warm vs cold interview styles
  - Check in at major milestones (e.g., once you’re done taking requirements, or after you’re done with the high-level design)
  - <img width="1177" alt="Screenshot 2024-11-28 at 9 59 15 PM" src="https://github.com/user-attachments/assets/c399587e-0f34-431d-b7c9-05997dd8050e">
  - SQL is preferred if it is more important that customers using your service always see up-to-date information, even if sometimes there is a slight delay.
  - Put simply, SQL databases are slower for writing than NoSQL databases due to the way data is stored. In contrast to this, NoSQL databases typically have slower reads
  - ![image](https://github.com/user-attachments/assets/902c0ed3-a60d-4334-a933-d76b019fbd9c)



- Reviewed more on booking systems https://www.greatfrontend.com/questions/system-design/travel-booking-airbnb
- Happy Thanksgiving :)

---

### Day 65: November 29, 2024 - Friday

#### Todays's Progress

✅ BANKI <br>
✅ Practice figjam <br>

#### Thoughts

- Reviewed another high level system design for frontend video, very good
- Reviewed basic concepts
- Praticed a few booking systems on figjam
- Prepped STAR format answers for experiences
- Pt 3 of interviewing.io
  - <img width="730" alt="Screenshot 2024-11-29 at 8 28 23 PM" src="https://github.com/user-attachments/assets/ab2c2171-c3d4-4a32-bc3b-45b4cbb059be">
  - <img width="730" alt="Screenshot 2024-11-29 at 8 30 16 PM" src="https://github.com/user-attachments/assets/02776dd0-7cad-4a61-ae0e-2ed57181bfe2">
  - <img width="730" alt="Screenshot 2024-11-29 at 8 30 44 PM" src="https://github.com/user-attachments/assets/c5fedda0-5933-464b-b45f-90c7d73db1ee">
  - <img width="1030" alt="Screenshot 2024-11-29 at 8 50 01 PM" src="https://github.com/user-attachments/assets/2208fec7-1547-4cde-b76d-ff6e28b144be">
  - <img width="816" alt="Screenshot 2024-11-29 at 9 16 47 PM" src="https://github.com/user-attachments/assets/2d047f1e-1f55-42c5-af45-e530a705731f">
  - Wow this is a great explanation of polling / websockets <img width="816" alt="Screenshot 2024-11-29 at 9 20 19 PM" src="https://github.com/user-attachments/assets/d2b8de3a-5de5-4267-8c87-7535df74ce26"><img width="816" alt="Screenshot 2024-11-29 at 9 20 57 PM" src="https://github.com/user-attachments/assets/8f2fc2e5-14e4-4326-8701-c6edff0d3a65">

  - Great article, will have to re-read over some parts bc they just flew over my head but love the resources at the end

---

### Day 66: November 30, 2024 - Saturday

#### Todays's Progress

✅ BANKI <br>
✅ Review System Design <br>
✅ Practice figjam <br>

#### Thoughts

- Great resource, especially on API Design: https://frontendlead.com/system-design/frontend-system-design-interview-guide
- Another great resource for system design: https://bytebytego.com/courses/system-design-interview/scale-from-zero-to-millions-of-users
- https://frontendmastery.com/posts/frontend-system-design-interview-guide/: <img width="733" alt="Screenshot 2024-11-30 at 12 06 39 PM" src="https://github.com/user-attachments/assets/829e9284-2807-4867-ae7a-1dfa47a2e708">
- mindmap: https://www.youtube.com/watch?v=JhcW0fuR_ig 
- <img width="1181" alt="Screenshot 2024-11-30 at 2 32 39 PM" src="https://github.com/user-attachments/assets/5f1a8b37-a6ad-4104-b15c-12df9ecfe301">
- <img width="712" alt="Screenshot 2024-11-30 at 2 38 26 PM" src="https://github.com/user-attachments/assets/0ad987f0-287b-4e2e-825e-19269b0879e1">
- Pretty cool resource for questions - https://www.techprep.app/full-stack
- So far there is a lot of "fullstack/backend" system design interviews on youtube, but I'm not really seeing any good frontend ones. There's a lot of content out there (greatfrontend, frontend lead) but I would love to see a video walkthrough to gain a better understanding on time management. [frontend-engineer](https://www.youtube.com/watch?v=LEaiGjffLEs) on youtube does frontend content but the diagrams etc are already pre-done for the video. I feel like if you were to start going into the level of detail on UI he does, that would take up a big chunk of time so it's not a true mock interview. Makes me think of making a video! 
- Also maybe this is just a personal opinion, but being someone who loves frontend aka visualization, it's interesting that I'm not seeing this. ALL the vids I'm seeing go from functional requirements right into api calls/data modeling/architecting. I have yet to see an approach from a user perspective like it's talked about in [frontendmastery](https://frontendmastery.com/posts/frontend-system-design-interview-guide/). When I think about designing fantastic realms, we started off with user stories which helped design a high level overview of the core features for mvp. This is how my brain understands things - going from a top down level. The vids I've been seeing jump straight to API's and data models which probably makes sense for a backend person bc that's how they see things - in data, but I see components, and think how users interact with them, THEN think about the data layer.
- I will say I did pick up some cool tidbits on how to better use figjam though! Like mindmapping the functional reqs, breaking each feature/ui into its own section
- Just food for thought. Going to record myself and see how it goes :) 

---

### Day 67: December 1, 2024 - Sunday

#### Todays's Progress

✅ BANKI <br>
✅ Mock Interview <br>

#### Thoughts

- Mock interview over yoga studio booking system, went well then spent time perfecting it and going over all my talking points
- Practice practice practice BANKI questions

---

### Day 68: December 2, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Interview 1 <br>
✅ Interview 2 <br>

#### Thoughts

- Whew it's been a long day. Good interviews though, feeling good about both. I can't believe how proud I am with myself. 0 experience of leetcode to solving a leetcode medium coding assessment to my first system design interview. LOTS OF PREP and it was worth it. I know I tried my best so I can only hope for the best. And still kill it tomorrow! 

---

<!---

### Day 69: December 3, 2024 - Tuesday

#### Todays's Progress

✅ ANKI <br>
✅  <br>
✅  <br>

#### Thoughts

-

---

### Day 70: December 4, 2024 - Wednesday

#### Todays's Progress

✅ Mentee Call <br>
✅  <br>

#### Thoughts

-

---

### Day 71: December 5, 2024 - Thursday

#### Todays's Progress

✅ Commit Your Code Conference <br>

#### Thoughts

-

---

### Day 72: December 6, 2024 - Friday

#### Todays's Progress

✅ Commit Your Code Conference <br>

#### Thoughts

-

---

### Day 73: December 7, 2024 - Saturday

#### Todays's Progress

✅ ANKI <br>
✅  <br>
✅  <br>

#### Thoughts

-

---
--->
