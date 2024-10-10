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
  - 10/10 timelapse of journey
  - 10/11 community involvement
  - 10/12 tech stack, socials / where to find or contact me, glimpse of projects (shown as cards)
  - 10/13 blog
  - 10/14 blog

---

<!---

### Day 1: October 9, 2024 - Monday

#### Todays's Progress

✅ ANKI <br>
✅ Huntober <br>

#### Thoughts

-



---

--->
