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

<!---
### Day 1: September 9, 2024 - Monday

#### Todays's Progress

✅ Daily Codewars <br>
✅ Daily CSSBattle <br>

#### Thoughts

-

---

--->
