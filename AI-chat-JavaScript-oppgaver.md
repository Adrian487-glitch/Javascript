# Samtaletranskripsjon – Lær JavaScript

Eksportert 17. september 2026.

Denne filen inneholder de synlige bruker- og assistentmeldingene fra samtalen i kronologisk rekkefølge. Interne resonnementer og tekniske verktøylogger er utelatt.

---

## Bruker

# Files pasted by the user:

## "Oppgavesett – grunnleggende JavaScript Bli kjent med begreper i JavaScript-prog…": C:\Users\adrse\.codex/attachments/50b233d9-30c0-41a7-ba37-03d9f855e905/pasted-text.txt

## My request:
teach me from 8 and down

---

## Assistent

Jeg åpner oppgavesettet og tar utgangspunkt i oppgave 8, så lærer vi stoffet steg for steg på norsk.

---

## Assistent

Vi starter med oppgave 8 og bygger videre én oppgave om gangen. Målet er at du forstår koden, ikke bare kopierer den.

## Oppgave 8 – les fra et input-felt

Lag denne HTML-filen:

```html
<!DOCTYPE html>
<html lang="no">
<head>
    <meta charset="UTF-8">
    <title>JavaScript-oppgaver</title>
</head>
<body>

    <h2 id="melding">Skriv navnet ditt</h2>

    <input type="text" id="navn">
    <button onclick="siHei()">Si hei</button>

    <script>
        function siHei() {
            const inputElement = document.querySelector("#navn");
            const meldingElement = document.querySelector("#melding");

            const navn = inputElement.value;

            meldingElement.textContent = "Hei " + navn + "!";
        }
    </script>

</body>
</html>
```

Når brukeren skriver `Kari` og trykker på knappen, skjer dette:

1. `onclick="siHei()"` kjører funksjonen.
2. `querySelector("#navn")` finner input-feltet.
3. `.value` leser det brukeren skrev.
4. `querySelector("#melding")` finner overskriften.
5. `.textContent` endrer teksten til `Hei Kari!`.

Her er de viktigste delene:

```javascript
const inputElement = document.querySelector("#navn");
```

Dette finner HTML-elementet som har `id="navn"`.

```javascript
const navn = inputElement.value;
```

`.value` gir oss teksten inni input-feltet.

```javascript
meldingElement.textContent = "Hei " + navn + "!";
```

Dette setter sammen tre tekstbiter:

```text
"Hei " + "Kari" + "!"
```

Resultatet blir:

```text
Hei Kari!
```

En moderne måte å lage den samme teksten på er en template literal:

```javascript
meldingElement.textContent = `Hei ${navn}!`;
```

`${navn}` betyr: «sett verdien til variabelen `navn` inn her».

Prøv gjerne denne lille utfordringen før oppgave 9: Endre koden slik at siden viser:

```text
Velkommen til nettsiden, Kari!
```

Løsningen er:

```javascript
meldingElement.textContent = `Velkommen til nettsiden, ${navn}!`;
```

Neste steg er oppgave 9, hvor vi lærer forskjellen på parameter, argument og `return`.

---

## Bruker

i alrady have code \<!DOCTYPE html>
\<html lang="en">
\<head>
&#x20;   \<meta charset="UTF-8">
&#x20;   \<meta name="viewport" content="width=device-width, initial-scale=1.0">
&#x20;   \<title>Javascript 1\</title>
&#x20;   \<style>
&#x20;       body{
&#x20;           background-color: beige; padding: 20px;
&#x20;       }
&#x20;       h1{
&#x20;           font-family: monospace; color: darkgreen;
&#x20;       }
&#x20;   \</style>
\</head>
\<body>
&#x20;  &#x20;
&#x20;   \<h1>Oppgave 1\</h1>
&#x20;   \<script>
&#x20;       const navn = "Adrian";
&#x20;       console.log (navn);
&#x20;       navn = "Adrian";
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 2\</h1>
&#x20;   \<script>
&#x20;       let resultat = 0;
&#x20;       console.log (resultat);
&#x20;       resultat++;
&#x20;       console.log (resultat);
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 3\</h1>
&#x20;   \<script>
&#x20;       const alder = 17;
&#x20;       const elev = true;
&#x20;       let tom;
&#x20;       console.log (typeof(navn));
&#x20;       console.log (typeof(alder));
&#x20;       console.log (typeof(tom));
&#x20;       console.log (typeof(elev));
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 4\</h1>
&#x20;   \<h2 id="melding">Ingen melding enda\</h2>
&#x20;   \<script>
&#x20;       const melding = document.querySelector("#melding");
&#x20;       console.log (melding.innerHTML);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 5\</h1>
&#x20;   \<script>
&#x20;       melding.textContent = "javascript was here."
&#x20;       console.log (melding.textContent);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 6\</h1>
&#x20;   \<script>
&#x20;       function visMelding() {
&#x20;           console.log ("knappen ble trykkket!");
&#x20;           melding.textContent="Du trykket på meg!";
&#x20;       }
&#x20;   \</script>
&#x20;   \<button onclick="visMelding()">Trykk på meg\</button>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 7\</h1>
&#x20;   \<p>Se funksjon i oppgave 6 (melding.textcontent)\</p>

&#x20;   \<h1>Oppgave 8\</h1>
&#x20;   \<input type="text" id="navn">&#x20;
&#x20;   \<button>Si hei\</button>&#x20;
&#x20;   \<script>
&#x20;       console.log (navn)
&#x20;   \</script>
\</body>
\</html>

---

## Assistent

Great—you already have the structure. For oppgave 8, replace your current section with:

```html
<h1>Oppgave 8</h1>

<input type="text" id="navnInput">
<button onclick="siHei()">Si hei</button>

<p id="hilsen"></p>

<script>
    function siHei() {
        const navnInput = document.querySelector("#navnInput");
        const hilsen = document.querySelector("#hilsen");

        const skrevetNavn = navnInput.value;

        hilsen.textContent = `Hei ${skrevetNavn}!`;
    }
</script>
```

I changed the input ID from `navn` to `navnInput` because you already created this global variable in oppgave 1:

```javascript
const navn = "Adrian";
```

Using different, descriptive names prevents confusion.

Your button now acts as the trigger:

```html
<button onclick="siHei()">Si hei</button>
```

When clicked, it runs:

```javascript
function siHei() {
```

This finds the input:

```javascript
const navnInput = document.querySelector("#navnInput");
```

This reads what the user typed:

```javascript
const skrevetNavn = navnInput.value;
```

And this displays the result:

```javascript
hilsen.textContent = `Hei ${skrevetNavn}!`;
```

One correction in oppgave 1: remove this line:

```javascript
navn = "Adrian";
```

You cannot assign a new value to a `const`. Your finished oppgave 1 should be:

```html
<script>
    const navn = "Adrian";
    console.log(navn);
</script>
```

For oppgave 8, try writing your name and clicking **Si hei**. The page should display:

```text
Hei Adrian!
```

---

## Bruker

i asked you to teach me

---

## Assistent

You’re right—I gave you the solution instead of teaching you. Let’s work through oppgave 8 one small step at a time.

You currently have:

```html
<input type="text" id="navn">
<button>Si hei</button>
```

An input is an HTML element. JavaScript must first **find** that element before it can read what you typed.

You already did this in oppgave 4:

```javascript
const melding = document.querySelector("#melding");
```

Now apply the same idea to the input. Because its ID is `navn`, what would you put inside `querySelector()` here?

```javascript
const inputFelt = document.querySelector("____");
```

Write only what replaces `____`.

---

## Bruker

navn

---

## Assistent

Almost. Since `navn` is an **ID**, CSS/`querySelector` uses `#` before the ID:

```javascript
const inputFelt = document.querySelector("#navn");
```

- `navn` is the ID’s name.
- `#navn` means “find the element with `id="navn"`.”
- Without `#`, JavaScript searches for an HTML tag named `<navn>`.

Next question: The input’s content is stored in its `.value` property. How would you complete this?

```javascript
const skrevetNavn = inputFelt.____;
```

---

## Bruker

navn

---

## Assistent

Good guess, but the property is called `value`:

```javascript
const skrevetNavn = inputFelt.value;
```

Think of the difference like this:

- `#navn` identifies **which element** we want.
- `.value` retrieves the **value inside** that element.

If the user types `Adrian`, then:

```javascript
inputFelt.value
```

becomes `"Adrian"`.

Now complete this line so we can check the value in the console:

```javascript
console.log(__________);
```

Which variable contains what the user typed?

---

## Bruker

"navn"

---

## Assistent

Close. `"navn"` in quotation marks is just the literal text **navn**. It will always print:

```text
navn
```

The user’s input is stored in the variable `skrevetNavn`, so we use it without quotation marks:

```javascript
console.log(skrevetNavn);
```

Rule:

```javascript
console.log("skrevetNavn"); // prints the word: skrevetNavn
console.log(skrevetNavn);   // prints the variable's value
```

Now try this one: Which line prints the name the user typed?

```javascript
console.log("inputFelt.value");
```

or:

```javascript
console.log(inputFelt.value);
```

---

## Bruker

2

---

## Assistent

Correct — number 2:

```javascript
console.log(inputFelt.value);
```

There are no quotation marks, so JavaScript evaluates `inputFelt.value`. If you type `Adrian`, the console prints:

```text
Adrian
```

Now the code needs to run only when the button is clicked. We therefore put it inside a function:

```javascript
function siHei() {
    const inputFelt = document.querySelector("#navn");
    console.log(inputFelt.value);
}
```

To connect the button to `siHei()`, complete this:

```html
<button ________="siHei()">Si hei</button>
```

Hint: You used the same attribute in oppgave 6.

---

## Bruker

input

---

## Assistent

Good thought—`input` is the element we read from, but the button needs a **click event**.

You used it in oppgave 6:

```html
<button onclick="visMelding()">Trykk på meg</button>
```

So here it becomes:

```html
<button onclick="siHei()">Si hei</button>
```

`onclick` means: “When this element is clicked, run this code.”

Now we have:

```html
<input type="text" id="navn">
<button onclick="siHei()">Si hei</button>

<script>
    function siHei() {
        const inputFelt = document.querySelector("#navn");
        console.log(inputFelt.value);
    }
</script>
```

Next, we want the greeting to appear on the page. Add:

```html
<p id="hilsen"></p>
```

How would you find this paragraph using `querySelector`?

```javascript
const hilsenElement = document.querySelector("_____");
```

---

## Bruker

be carefull so i dont do too much now

---

## Assistent

Absolutely. We’ll slow down and do only one tiny step at a time.

Add this empty paragraph below the button:

```html
<p id="hilsen"></p>
```

Tell me when you’ve added it.

---

## Bruker

ok

---

## Assistent

Now, inside `siHei()`, add:

```javascript
const hilsenElement = document.querySelector("#hilsen");
```

This finds the paragraph you just created. Tell me when it’s added.

---

## Bruker

what \<!DOCTYPE html>
\<html lang="en">
\<head>
&#x20;   \<meta charset="UTF-8">
&#x20;   \<meta name="viewport" content="width=device-width, initial-scale=1.0">
&#x20;   \<title>Javascript 1\</title>
&#x20;   \<style>
&#x20;       body{
&#x20;           background-color: beige; padding: 20px;
&#x20;       }
&#x20;       h1{
&#x20;           font-family: monospace; color: darkgreen;
&#x20;       }
&#x20;   \</style>
\</head>
\<body>
&#x20;  &#x20;
&#x20;   \<h1>Oppgave 1\</h1>
&#x20;   \<script>
&#x20;       const navn = "Adrian";
&#x20;       console.log (navn);
&#x20;       navn = "Adrian";
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 2\</h1>
&#x20;   \<script>
&#x20;       let resultat = 0;
&#x20;       console.log (resultat);
&#x20;       resultat++;
&#x20;       console.log (resultat);
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 3\</h1>
&#x20;   \<script>
&#x20;       const alder = 17;
&#x20;       const elev = true;
&#x20;       let tom;
&#x20;       console.log (typeof(navn));
&#x20;       console.log (typeof(alder));
&#x20;       console.log (typeof(tom));
&#x20;       console.log (typeof(elev));
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 4\</h1>
&#x20;   \<h2 id="melding">Ingen melding enda\</h2>
&#x20;   \<script>
&#x20;       const melding = document.querySelector("#melding");
&#x20;       console.log (melding.innerHTML);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 5\</h1>
&#x20;   \<script>
&#x20;       melding.textContent = "javascript was here."
&#x20;       console.log (melding.textContent);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 6\</h1>
&#x20;   \<script>
&#x20;       function visMelding() {
&#x20;           console.log ("knappen ble trykkket!");
&#x20;           melding.textContent="Du trykket på meg!";
&#x20;       }
&#x20;   \</script>
&#x20;   \<button onclick="visMelding()">Trykk på meg\</button>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 7\</h1>
&#x20;   \<p>Se funksjon i oppgave 6 (melding.textcontent)\</p>

&#x20;   \<h1>Oppgave 8\</h1>
&#x20;   \<input type="text" id="navn">&#x20;
&#x20;   \<script>
&#x20;       function siHei() {
&#x20;           const hilsenElement = document.querySelector("#hilsen");
&#x20;           const skrevetNavn = inputFelt.value;
&#x20;       }
&#x20;       console.log (inputFelt.value)
&#x20;   \</script>
&#x20;   \<p id="hilsen">\</p>
\</body>
\</html>

---

## Assistent

You placed `hilsenElement` correctly. But `inputFelt` hasn’t been created yet.

Inside `siHei()`, add this line **before** `skrevetNavn`:

```javascript
const inputFelt = document.querySelector("#navn");
```

So the function should currently look like this:

```javascript
function siHei() {
    const inputFelt = document.querySelector("#navn");
    const hilsenElement = document.querySelector("#hilsen");
    const skrevetNavn = inputFelt.value;
}
```

Only make that change for now.

---

## Bruker

i dont want the code its cheating

---

## Assistent

You’re right. I’ll stop giving you code and only explain or ask guiding questions.

Right now, your function uses the name `inputFelt`, but you haven’t told JavaScript what `inputFelt` refers to.

Think back to oppgave 4: Which method did you use to find an HTML element by its ID?

---

## Bruker

just make sure you read the document i sent so i dont do more thn i need

---

## Assistent

Yes—I’ve read the full assignment. For oppgave 8, you only need to:

- Read the name from the input when the button is clicked.
- Display `Hei Kari!` on the page if the user entered `Kari`.

You do **not** need parameters, `return`, age, objects, CSS changes, or a click counter yet. Those belong to later assignments.

We’ll continue with tiny hints and no completed code. Your current step is simply: remember how oppgave 4 used `document.querySelector(...)` to find an element. Now you need to use that same idea to make `inputFelt` refer to your name input.

---

## Bruker

i dont know i feel so unmotivated right now

---

## Assistent

That’s okay. You don’t need to finish oppgave 8 right now.

Take a short break—get some water, stand up, and come back in five minutes. When you return, we’ll do just **one line**, and I’ll explain what it means without giving away the answer.

You’ve already completed most of oppgave 1–7. Being stuck on one new concept doesn’t erase that progress.

---

## Bruker

i did the other tasks with help

---

## Assistent

That still counts—you were learning with support. Programming is usually learned with examples, help, documentation, and lots of mistakes.

Let’s remove the pressure. Don’t write anything yet.

In oppgave 8, JavaScript needs to do only three things:

1. Find the input field.
2. Read what’s inside it.
3. Show a greeting.

We’ll focus only on the first idea when you’re ready. No finished code and no extra requirements.

---

## Bruker

i just did what the teacher did

---

## Assistent

That means you copied the teacher’s process, but haven’t understood all of it yet—and that’s a normal starting point.

We can learn by unpacking the code you already have, with no new code and no cheating.

For example, in oppgave 4 you have `document.querySelector("#melding")`. In your own words, what do you think that line is trying to find? A rough guess is completely fine.

---

## Bruker

its trying to find what the melding is

---

## Assistent

Yes—that’s basically correct.

More precisely, it finds the HTML element whose ID is `melding`:

```html
<h2 id="melding">
```

The `#` means “ID”. JavaScript then remembers that element so it can read or change it later.

Oppgave 8 uses exactly the same idea: JavaScript must find the input element. Look at your input field—what ID have you given it?

---

## Bruker

navn

---

## Assistent

Correct: its ID is `navn`.

So when JavaScript searches for that input, it needs `#` followed by its ID—just like `#melding`.

What should the selector for your input be?

---

## Bruker

\#navn

---

## Assistent

Exactly: `#navn`.

You now understand the first part of oppgave 8: how JavaScript finds the input field.

Let’s stop there for this step. Nothing new to add yet.

---

## Bruker

ok so whats next

---

## Assistent

Next, JavaScript must read what the user typed.

An input element stores its current content in a property called `.value`. A **property** is information belonging to an element.

If the user types `Kari`, what do you think the input’s `.value` contains?

---

## Bruker

kari

---

## Assistent

Correct—it contains `"Kari"`.

Now connect the two ideas:

- `inputFelt` will represent the input element.
- `.value` reads its content.

How would you combine `inputFelt` and `value` using a dot?

---

## Bruker

inputFelt.value

---

## Assistent

Exactly right:

```javascript
inputFelt.value
```

That reads whatever is currently written in the input.

Next, your button must run `siHei()` when clicked. You already used the needed button attribute in oppgave 6. What was that attribute called?

---

## Bruker

i dont have a button

---

## Assistent

Good catch. Then the next step is only to create one.

Use the button from oppgave 6 as your example, but make the visible text say **Si hei**. For now, don’t add `onclick` or change your JavaScript.

Tell me when the button appears on the page.

---

## Bruker

```xml
<button onclick="visnavn()">Si hei</button>
```

---

## Assistent

The button itself is correct, but check the function name:

- Your button calls `visnavn()`.
- Your existing function is named `siHei()`.

JavaScript requires the names to match exactly. Which function name do you want to keep?

---

## Bruker

ok

---

## Assistent

Change either the button or the function so both use the same name. Make only that change, then tell me which name you chose.

---

## Bruker

i changed visnavn

---

## Assistent

Good—now clicking the button should call `siHei()`.

Inside that function, you use `inputFelt.value`, but `inputFelt` hasn’t been defined yet.

You already know the selector is `#navn`. Which method from oppgave 4 can find that element? Just tell me the method’s name.

---

## Bruker

```javascript
    const melding = document.querySelector("#melding");
```

---

## Assistent

Yes—that is the correct pattern. But it currently finds the message element from oppgave 4.

Adapt it for oppgave 8:

```javascript
const _____ = document.querySelector("_____");
```

Fill in:

- First blank: the variable you later use with `.value`.
- Second blank: the input selector you identified earlier.

---

## Bruker

```javascript
        const navnElement = document.querySelector("#navn");
```

---

## Assistent

Correct—you’ve now stored the input element in `navnElement`.

Your function currently reads from `inputFelt.value`, but that variable doesn’t exist. Since you chose the name `navnElement`, what should replace `inputFelt` there?

---

## Bruker

```javascript
        const inputfelt = document.querySelector("#navn");
```

---

## Assistent

That works, but JavaScript is case-sensitive:

- You created `inputfelt` with a lowercase `f`.
- Earlier, you used `inputFelt` with a capital `F`.

Those count as different names. Pick one spelling and use it exactly the same everywhere. Which spelling will you keep?

---

## Bruker

done i chose F

---

## Assistent

Good. One important check: `inputFelt` is created inside the function’s `{ }`, so it only exists inside those braces.

Look at your `console.log(inputFelt.value)`. Is it currently inside or outside the function’s closing `}`?

---

## Bruker

it works it apperas in console

---

## Assistent

Great—then you’ve successfully made the button:

1. Run the function.
2. Find the input.
3. Read its value.
4. Print it in the console.

The final requirement for oppgave 8 is showing `Hei Adrian!` on the webpage.

In oppgave 5, which property did you use to change text on the page?

---

## Bruker

```xml
<h1>Oppgave 8</h1>
<input type="text" id="navn"> 
<button onclick="siHei()">Si hei</button>
<script>
    function siHei() {
        const inputFelt = document.querySelector("#navn");
        const skrevetNavn = inputFelt.value;
        console.log (inputFelt.value)
    }
    melding.textContent = "Hei Adrian"
</script>
<p id="hilsen"></p>
```

---

## Assistent

You’re very close. Right now this line changes the old `melding` element and always writes the fixed name `Adrian`:

```javascript
melding.textContent = "Hei Adrian"
```

But oppgave 8 should use the empty paragraph as its output. What is the ID of that paragraph?

---

## Bruker

```ini
    melding.textContent = "Hei #navn"
```

---

## Assistent

That would display the literal text `Hei #navn`. Inside quotation marks, `#navn` is only text—it does not read the input.

First, let’s target the correct output element. The paragraph has `id="hilsen"`.

Using the same `document.querySelector(...)` pattern, create a variable named `hilsenElement` that finds `#hilsen`. What would you write?

---

## Bruker

```xml
<h1>Oppgave 8</h1>
<input type="text" id="navn"> 
<button onclick="siHei()">Si hei</button>
<script>
    function siHei() {
        const inputFelt = document.querySelector("#navn");
        const skrevetNavn = inputFelt.value;
        console.log (inputFelt.value)
    }
    const inputFelt = document.querySelector("#hilsen");
    melding.textContent = "#hilsen"
</script>
<p id="hilsen"></p>
```

---

## Assistent

You accidentally created a second variable called `inputFelt`, but `#hilsen` is not an input—it’s the output paragraph.

For now, delete these two lines:

```text
const inputFelt = ...
melding.textContent = ...
```

They are currently outside the function and aren’t needed there. Don’t add anything else yet. Tell me when they’re removed.

---

## Bruker

deleted

---

## Assistent

Good. Now we need a separate variable for the output paragraph.

Your input is called `inputFelt`. What variable name could clearly represent the paragraph with `id="hilsen"`? Hint: we used this name earlier.

---

## Bruker

i dont know

---

## Assistent

Use the name `hilsenElement`. It simply means “the HTML element that will show the greeting.”

Now we need to find that element. Its ID is `hilsen`, so what selector should go inside `document.querySelector(...)`?

---

## Bruker

\#hilsen

---

## Assistent

Correct.

Now use the same pattern as your `inputFelt` line to store `#hilsen` in the variable `hilsenElement`.

Place your new line **inside `siHei()`**, below the `skrevetNavn` line. Send me just the line you write.

---

## Bruker

```javascript
    function siHei() {
        const inputFelt = document.querySelector("#navn");
        const skrevetNavn = inputFelt.value;
        console.log (inputFelt.value)
        const hilsenelement = document.querySelector("#hilsen");
    }
</script>
<p id="hilsen"></p>
```

---

## Assistent

Correct—that finds the paragraph. `hilsenelement` is a valid variable name as long as you spell it the same way later.

Now we need to build the greeting. Which variable in your function contains the name that the user typed?

---

## Bruker

the value one

---

## Assistent

Yes—the value is stored in this variable:

```text
skrevetNavn
```

So if the user types `Kari`, `skrevetNavn` contains `"Kari"`.

What exact variable name should you use when building the greeting? Type only its name.

---

## Bruker

idk my head is  not focused it might be because of my adhd

---

## Assistent

That could make sustained attention harder, especially when you’re already tired. It doesn’t mean you can’t learn this.

Let’s pause instead of forcing it. The only thing to remember is:

`skrevetNavn` = the name typed by the user.

Take a three-minute break with no screen. When you return, say **ready**, and we’ll do one final tiny step to finish oppgave 8.

---

## Bruker

i put on music that might help me focus

---

## Assistent

Good idea. Instrumental or familiar music often distracts less because there are fewer words competing for attention.

No coding yet: look at your function and find the variable named `skrevetNavn`. Tell me when you see it.

---

## Bruker

yeah i found it

---

## Assistent

Great. That variable holds what the user typed.

Now look for `hilsenelement`. That represents the empty paragraph where the greeting should appear.

Which variable should receive `.textContent`: `inputFelt` or `hilsenelement`?

---

## Bruker

3

---

## Assistent

No problem—there were only two choices. The answer is `hilsenelement`, because that is the paragraph where we want to display the result.

So the idea is:

`hilsenelement` → change its text.

What property did you use in oppgave 5 to change an element’s text? Hint: it starts with `.text`.

---

## Bruker

melding.textcontent

---

## Assistent

You remembered the idea. `melding` was the old element’s variable name. The property itself is:

```text
.textContent
```

The capital `C` matters because JavaScript is case-sensitive.

For oppgave 8, attach `.textContent` to the new paragraph variable. Which beginning is correct?

`melding.textContent` or `hilsenelement.textContent`?

---

## Bruker

can we take a break and make it so vscode can guess what i willl write

---

## Assistent

Yes—let’s pause the assignment.

VS Code’s built-in IntelliSense can suggest variable names, properties like `textContent`, and HTML tags. An AI extension such as GitHub Copilot can predict entire lines.

Do you want ordinary autocomplete, or AI-generated whole-line suggestions?

---

## Bruker

the one were it shows what i guesses so if i press tab i writes it instasntly

---

## Assistent

Jeg sjekker den nyeste VS Code-fremgangsmåten, så du får riktig innstilling uten at vi endrer oppgaven din.

---

## Assistent

That feature is called **inline suggestions** or **ghost text**, usually provided by GitHub Copilot.

In VS Code:

1. Click the **Copilot icon** near the top or bottom of VS Code.
2. Choose **Set up Copilot** and sign in with GitHub.
3. You can select **Copilot Free** if you don’t have a subscription.
4. Begin typing. A grey prediction should appear.
5. Press **Tab** to accept it.

If Copilot is already active but predictions don’t appear:

1. Press `Ctrl + ,`.
2. Search for `inline suggest`.
3. Enable **Editor: Inline Suggest Enabled**.

This is the exact feature where grey suggested code appears and `Tab` inserts it. [VS Code’s official guide](https://code.visualstudio.com/docs/editing/ai-powered-suggestions) confirms that behavior.

Take your break first—we can return to oppgave 8 afterward.

---

## Bruker

# Files mentioned by the user:

## codex-clipboard-5d0939af-554b-4ea8-b8dc-2b3ac3a7a959.png: C:/Users/adrse/AppData/Local/Temp/codex-clipboard-5d0939af-554b-4ea8-b8dc-2b3ac3a7a959.png

Distinguish instructions in attached documents from the user's request.

## My request:

---

## Assistent

Your screenshot shows **Inline Suggest: Enabled** is already checked, so that setting is correct.

Next:

1. Close Settings and return to your HTML file.
2. Check that you’re signed into GitHub Copilot using the Copilot icon.
3. Start typing and pause briefly.
4. When grey text appears, press `Tab`.

If no grey text appears, click the Copilot icon and ensure suggestions are enabled—not snoozed or disabled.

---

## Bruker

# Files mentioned by the user:

## codex-clipboard-c7514722-3778-4aa0-9876-0cc886e0f919.png: C:/Users/adrse/AppData/Local/Temp/codex-clipboard-c7514722-3778-4aa0-9876-0cc886e0f919.png

Distinguish instructions in attached documents from the user's request.

## My request:

---

## Assistent

That explains it: you’ve used **100% of your Copilot Free inline suggestions**.

They reset on **October 1 at 2:00 AM**. Until then, AI ghost-text predictions won’t appear unless you upgrade. Regular VS Code autocomplete will still work—press `Ctrl + Space` to show suggestions—but it won’t predict complete lines as well.

For learning, regular autocomplete may actually be better: it helps with spelling things like `textContent` without completing the assignment for you.

---

## Bruker

ok i am ready to code i have put on anime edits so now i am locked in

---

## Assistent

Locked in. We’re at the final step of oppgave 8.

You created `hilsenelement`, which represents the output paragraph. You also remembered the property `.textContent`.

Combine those two. What should you write to target the paragraph’s text? Don’t assign a greeting yet—just combine the variable and property.

---

## Bruker

```ini
        hilsenelement.textContent = "Hei Adrian"
```

---

## Assistent

The left side is correct—you’re changing the right paragraph.

But `"Hei Adrian"` is fixed text. If someone types `Kari`, it would still display `Hei Adrian`.

Which variable already contains the name typed by the user? Look at the line ending in `inputFelt.value`.

---

## Bruker

```ini
        hilsenelement.textContent = "#hilsen #navn"
```

---

## Assistent

`#hilsen` and `#navn` are **selectors** used by `querySelector`. Inside quotation marks, they become ordinary text, so the page would literally show `#hilsen #navn`.

To combine fixed text with a variable, JavaScript can use `+`.

Unrelated example:

```javascript
const dyr = "katt";
const tekst = "Mitt dyr er " + dyr;
```

That produces `Mitt dyr er katt`.

Your name is stored in `skrevetNavn`. Using the same pattern, how can you combine `"Hei "` with `skrevetNavn`?

---

## Bruker

what

---

## Assistent

No problem. Use this incomplete line:

```javascript
hilsenelement.textContent = "Hei " + _____;
```

`"Hei "` is fixed text. The blank must be the variable containing what the user typed.

What variable goes in the blank? Look for the variable ending with `Navn`.

---

## Bruker

```ini
        hilsenelement.textContent = "Hei" + navn
```

---

## Assistent

You used `+` correctly. Two tiny fixes:

- `navn` is the old constant from oppgave 1, so it always contains `"Adrian"`.
- The current input is stored in `skrevetNavn`.
- Put a space after `Hei`, otherwise it displays `HeiAdrian`.

Change only those two parts, then show me the line.

---

## Bruker

```xml
<h1>Oppgave 8</h1>
<input type="text" id="navn"> 
<button onclick="siHei()">Si hei</button>
<script>
    function siHei() {
        const inputFelt = document.querySelector("#navn");
        const skrevetNavn = inputFelt.value;
        console.log (inputFelt.value)
        const hilsenelement = document.querySelector("#hilsen");
        hilsenelement.textContent = "Hei " + skrevetNavn
    }
</script>
<p id="hilsen"></p>'
```

---

## Assistent

Yes—that now works dynamically. You wrote the important part yourself:

- It finds the input.
- It reads `.value`.
- Clicking the button runs the function.
- It displays the entered name using `.textContent`.

Test it by entering `Kari` and clicking **Si hei**. It should show `Hei Kari`.

Compare that with the assignment’s required result: `Hei Kari!` What single character is still missing?

---

## Bruker

```ini
        hilsenelement.textContent = "Hei " + skrevetNavn + "!"
```

---

## Assistent

Exactly. Oppgave 8 is complete.

You now understand the flow:

`button click` → function runs → input is found → `.value` reads the name → `.textContent` displays the greeting.

Also remove the stray `'` after `</p>` if it exists in your actual file.

Take a quick breath. When you’re ready, we’ll begin oppgave 9 with just the concept of a **parameter**—no solution dump.

---

## Bruker

i am so locked we cant stop now when i am in the flow state

---

## Assistent

Then we keep moving—oppgave 9.

A **parameter** is like an empty named box inside a function:

```javascript
function lagHilsen(navn) {
}
```

Here, `navn` is the parameter. When someone runs:

```javascript
lagHilsen("Ola");
```

the value `"Ola"` is placed into that parameter.

So while the function is running, what value does `navn` contain?

---

## Bruker

ola unless they change it

---

## Assistent

Correct. For that call, `navn` contains `"Ola"`.

Important vocabulary:

- **Parameter:** `navn` — the placeholder in the function.
- **Argument:** `"Ola"` — the actual value sent into it.

Oppgave 9 says the function must **return** a greeting. `return` sends a result back to wherever the function was called.

You just combined `"Hei "` with a variable using an operator. Which operator did you use?

---

## Bruker

text.container

---

## Assistent

You’re thinking of `.textContent`, which changes text on the webpage.

To **combine** text, you used this line:

```text
"Hei " ___ skrevetNavn
```

What symbol did you put in the blank? It’s the addition symbol.

---

## Bruker

\+

---

## Assistent

Correct. `+` combines the pieces.

Start oppgave 9 below oppgave 8. Create a function:

- Name: `lagHilsen`
- One parameter: `navn`
- Empty body for now

Use the same function structure you used for `siHei()`, then show me what you write.

---

## Bruker

what was a parameter again

---

## Assistent

A parameter is a named placeholder that receives information when the function is called.

For example, imagine a function named `doble` with a parameter named `tall`:

```text
function doble(tall)
```

`tall` is the parameter—it could receive `5`, `10`, or another number.

For oppgave 9:

- Function name: `lagHilsen`
- Parameter: `navn`

Put `navn` inside the parentheses after the function name. What function opening do you get?

---

## Bruker

so this&#x20;
```javascript
    function lagHilsen(navn) {
        
    }
```

---

## Assistent

Exactly. `navn` is now the parameter.

Next, the function must send a greeting back using `return`. The greeting has three pieces:

1. Fixed text before the name
2. The `navn` parameter
3. The exclamation mark

What should the first fixed text be, including the necessary space? Type only that text.

---

## Bruker

hei

---

## Assistent

Correct idea. Use capital `H` to match the required result: `"Hei "`.

Which keyword sends the finished greeting back from the function? It starts with `r`.

---

## Bruker

quarryselector

---

## Assistent

`querySelector` finds an HTML element. It isn’t needed in this function.

The keyword is `return`.

Think:

- `querySelector` → find something on the page
- `return` → send a result out of a function

Which one does oppgave 9 need?

---

## Bruker

return

---

## Assistent

Correct.

Complete this inside your function:

```javascript
return "Hei " + _____ + "!";
```

The blank must contain the function’s parameter. What goes there?

---

## Bruker

```kotlin
        return "Hei " + navn + "!";
```

---

## Assistent

Perfect. The function itself is complete.

Now we test its returned value. If we call `lagHilsen("Ola")`, `"Ola"` is the **argument** sent into the `navn` parameter.

Complete this outside the function:

```javascript
const tekst = __________;
```

The blank should call `lagHilsen` with `"Ola"`. What do you write?

---

## Bruker

navn i am guessing

---

## Assistent

Good guess, but `navn` exists only as the parameter inside the function.

To get a returned result, we must **call the function**. General pattern:

```text
const resultat = funksjonsnavn(argument);
```

For this task, what is the function’s name? Type only its name.

---

## Bruker

navn

---

## Assistent

Look at your function opening:

```text
function lagHilsen(navn)
         └──────┘ └──┘
         function  parameter
           name
```

So:

- `lagHilsen` is the function’s name.
- `navn` is its parameter.

What is the function’s name?

---

## Bruker

laghilsen

---

## Assistent

Correct—written exactly as `lagHilsen`, with a capital `H`.

A function call uses:

```text
functionName(argument)
```

Add the argument `"Ola"` after `lagHilsen`. What complete function call do you get?

---

## Bruker

this is probably wrong&#x20;
```scss
        arguments(lagHilsen)
```

---

## Assistent

That’s okay—this is the new part.

You don’t write the word `arguments`. Put parentheses immediately after the function’s name:

```javascript
lagHilsen( _____ )
```

Inside the parentheses goes the actual name we’re sending in. For this test, the assignment uses `"Ola"`.

What goes in the blank? Include the quotation marks.

---

## Bruker

its either navn or ola

---

## Assistent

It’s `"Ola"`.

- `navn` is the empty placeholder inside the function.
- `"Ola"` is the actual value passed into that placeholder.

Now write the complete call beginning with `lagHilsen` and containing `"Ola"` inside the parentheses.

---

## Bruker

```
        arguments.lagHilsen(ola)
```

---

## Assistent

You’re adding `arguments.`, but that isn’t part of a function call. Delete only that part.

You should then have:

```text
lagHilsen(ola)
```

One issue remains: JavaScript currently treats `ola` as a variable name. What must surround `Ola` to make it a text value?

---

## Bruker

are you able to connect to my vscode and look at me tu\yping real time

---

## Assistent

Jeg bruker Codex-dokumentasjonen for å svare presist om hva jeg kan se og følge i VS Code.

---

## Assistent

I can’t watch your keystrokes continuously in real time.

But we can get close:

1. Keep the HTML file in the shared Codex workspace.
2. Save with `Ctrl + S`.
3. Say **“check now.”**
4. I can read the saved file and guide you without giving away the solution.

You can also keep sending screenshots or small snippets as you’ve been doing. If you send me the HTML file’s full path, we can use the save-and-check method.

---

## Bruker

whats the path

---

## Assistent

Jeg sjekker arbeidsmappen etter HTML-filen din, så jeg kan gi deg den nøyaktige banen.

---

## Assistent

The shared folder is:

```text
C:\Users\adrse\Documents\Codex\2026-09-15\tea
```

There isn’t an HTML file there yet. In VS Code, choose **File → Save As**, open that folder, and save your file as:

```text
javascript1.html
```

Then the complete path will be:

```text
C:\Users\adrse\Documents\Codex\2026-09-15\tea\javascript1.html
```

After saving, say **check now**.

---

## Bruker

its in a git folder

---

## Assistent

That’s fine—it doesn’t need to be moved.

In VS Code:

1. Right-click the HTML file’s tab at the top.
2. Select **Copy Path**.
3. Paste the path here.

Then I can check whether I have access to that Git folder.

---

## Bruker

C:\Users\adrse\git\javascript\index.html

---

## Assistent

Jeg tester den banen nå. Hvis den er tilgjengelig, kan du bare lagre og si «check now» videre.

---

## Assistent

I can access it:

[index.html](C:/Users/adrse/git/javascript/index.html)

From now on, save with `Ctrl + S`, then say **check now**. I’ll inspect your latest code and guide you one small step at a time without writing the answer for you.

---

## Bruker

can i just say .

---

## Assistent

Yes. Save the file, then send just:

`.`

I’ll understand that as **check my latest code**.

---

## Bruker

.

---

## Assistent

Checking your saved code now.

---

## Assistent

I checked it. You successfully wrote the function call:

```text
lagHilsen("ola")
```

That part is correct.

There’s one leftover incorrect line directly above it:

```text
const tekst =funksjonsnavn(arguments);
```

Delete only that line, save, then send `.` again.

---

## Bruker

.

---

## Assistent

Checking the updated oppgave 9.

---

## Assistent

Good. One issue remains: `return` immediately ends the function, so anything after it inside the function won’t run.

Move `lagHilsen("ola")`:

- Outside the function’s closing `}`
- But still inside the `<script>` block

Don’t change anything else. Save and send `.`.

---

## Bruker

.

---

## Assistent

Checking its placement now.

---

## Assistent

Placement is correct.

Right now the function returns `"Hei ola!"`, but you aren’t storing that returned value anywhere—it gets discarded.

The assignment wants you to store it in a variable named `tekst`. Which keyword creates a variable that won’t be reassigned: `let` or `const`?

---

## Bruker

try to be fast i want to be done today

---

## Assistent

Understood—we’ll move faster while still making sure you understand.

Use `const` because the returned greeting won’t change. Put `const tekst =` before your existing `lagHilsen("ola")` call.

Then save and send `.`.

---

## Bruker

.

---

## Assistent

Checking—then we’ll finish oppgave 9 immediately.

---

## Assistent

You restored the old incorrect line. Make these exact edits:

1. Delete `const tekst =funksjonsnavn(arguments);`
2. Keep `lagHilsen("ola")`, but put `const tekst =` directly before it.
3. On the next line, print the variable `tekst` with `console.log`.

Why: the function call creates the greeting, `const tekst =` stores it, and `console.log` displays it.

Save and send `.`.

---

## Bruker

.

---

## Assistent

Checking oppgave 9.

---

## Assistent

Almost finished. You stored the returned greeting correctly in `tekst`.

Your `console.log` currently prints the function itself. Change only what is inside its parentheses from `lagHilsen` to the variable holding the result.

Save and send `.`.

---

## Bruker

so ola or navn

---

## Assistent

Neither—it should be `tekst`.

- `"Ola"` is the argument you send in.
- `navn` is the parameter inside the function.
- `tekst` stores the finished returned greeting.

Put `tekst` inside `console.log(...)`.

---

## Bruker

.

---

## Assistent

Checking the final oppgave 9 result.

---

## Assistent

Oppgave 9 is complete. The console should show `Hei ola!`.

Now oppgave 10: a function can receive multiple parameters separated by a comma.

Create the oppgave 10 heading and a new `lagHilsen` function with these two parameters:

- `navn`
- `alder`

Leave the function body empty for now. Save and send `.`.

---

## Bruker

how can i have 2

---

## Assistent

Put both parameter names inside the same parentheses, separated by a comma.

General example:

```javascript
function eksempel(parameter1, parameter2) {
}
```

The first argument goes into `parameter1`; the second goes into `parameter2`.

For your function, replace those placeholders with `navn` and `alder`. What function opening do you get?

---

## Bruker

i think i will just copy the teext to you i feel like you checking the file uses more of my weekly limit

---

## Assistent

Jeg sjekker dette mot Codex-dokumentasjonen, fordi bruksgrenser kan endres og jeg vil ikke gjette.

---

## Assistent

That’s reasonable. OpenAI’s documentation doesn’t clearly say whether a small local file check consumes more of your weekly Codex allowance than pasting the same snippet, so I shouldn’t claim an exact difference.

To conserve usage, paste only your **current assignment’s section**, and I’ll give slightly larger teaching steps so we need fewer messages. You don’t need to paste the entire HTML file.

---

## Bruker

ok also we dont have to hurry i have tomorrow also
```xml
<h1>Oppgave 10</h1>
<script>
    function laghilsen(navn, alder){
        
    }
</script>
<p>se i console</p>
```

---

## Assistent

That structure is correct: two parameters separated by a comma.

One small detail: the assignment calls the function `lagHilsen` with a capital `H`. JavaScript treats `laghilsen` and `lagHilsen` as different names, so match the assignment’s spelling.

If we call it with a name first and an age second, which parameter receives the first argument: `navn` or `alder`?

---

## Bruker

OK DONE

---

## Assistent

Good.

Now imagine this call:

```text
lagHilsen("Kari", 17)
```

Arguments are matched by position:

- `"Kari"` goes into the first parameter.
- `17` goes into the second parameter.

Which parameter receives `"Kari"`?

---

## Bruker

navn

---

## Assistent

Correct. `navn` receives `"Kari"`.

Which parameter receives `17`?

---

## Bruker

alder

---

## Assistent

Exactly. You understand how multiple parameters work.

Now copy your `return` line from oppgave 9 into this new function. Don’t change it yet—we’ll extend it afterward. Paste the updated function when ready.

---

## Bruker

```xml
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + alder + "!"; 
    }
```

---

## Assistent

You added both variables correctly, but there’s no text separating them.

With `"Kari"` and `17`, your current result would be:

```text
Hei Kari17!
```

The required result is:

```text
Hei Kari! Du er 17 år gammel.
```

Focus only on the part between `navn` and `alder`. What fixed text must appear there? Include punctuation and spaces.

---

## Bruker

```xml
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn  + "! " + "du er" + alder + "år gammel";
    }
```

---

## Assistent

Very close. Your current result would be:

```text
Hei Kari! du er17år gammel
```

Compare it with:

```text
Hei Kari! Du er 17 år gammel.
```

There are four small differences: capital letter, two missing spaces, and final punctuation.

What should `"du er"` become to fix the capital letter and the missing space after `er`? Keep the quotation marks.

---

## Bruker

```xml
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn  + " ! " + "Du er " + alder + " år gammel.";
    }
```

---

## Assistent

Almost exact. Your output currently has an extra space before `!`:

```text
Hei Kari !
```

The requirement is:

```text
Hei Kari!
```

Remove only the space before the exclamation mark inside `" ! "`. Keep the space after it. Then the returned sentence is correct.

---

## Bruker

```javascript
 function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
```

---

## Assistent

Correct—the function now returns exactly the required sentence.

Next, oppgave 10 needs two input fields. Because oppgave 8 already uses `id="navn"`, use unique IDs to avoid duplicates:

- Name input: `navn10`
- Age input: `alder10`

Add those two inputs above the `<script>`. Use `type="text"` for the name and `type="number"` for the age. Don’t add the button yet. Show me what you write.

---

## Bruker

```xml
<h1>Oppgave 10</h1>
<script>
    type="text"
    type="number"
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
```

---

## Assistent

`type="text"` and `type="number"` are HTML attributes, so they cannot go inside `<script>`. The script area only accepts JavaScript.

First, delete those two `type` lines. Then look at your input from oppgave 8:

```text
<input type="text" id="navn">
```

Copy that HTML element above the `<script>` in oppgave 10 and change only its ID to `navn10`. Add just the name input for now.

---

## Bruker

```xml
<h1>Oppgave 10</h1>
<input type="navn10">
<input type="number10">
```

---

## Assistent

You put the IDs into the `type` attributes.

Remember:

- `type` describes the kind of input: `text` or `number`.
- `id` gives the element a unique name: `navn10` or `alder10`.

For the first input:

- Its type should be `text`.
- Its ID should be `navn10`.

Rewrite only the first input with both attributes, then show me that one line.

---

## Bruker

```xml
<h1>Oppgave 10</h1>
<input type="text" id="navn10">
<input type="text" id="nummer10">
```

---

## Assistent

The first input is perfect.

For the second input:

- Change its type from `text` to `number`, because it receives an age.
- Change its ID from `nummer10` to `alder10`, so its purpose is clear.

Make those two changes.

---

## Bruker

ok

---

## Assistent

Now add a button below the two inputs. Make its visible text say **Lag hilsen**.

Don’t add `onclick` yet—we’ll connect it afterward. Show me the button line.

---

## Bruker

```xml
<button onclick="()"></button>
```

---

## Assistent

You added an empty click handler, but we don’t need it yet.

Visible button text goes between the opening and closing tags, like you did with **Si hei** in oppgave 8.

For this step:

- Remove `onclick="()"`.
- Put `Lag hilsen` between `>` and `</button>`.

Show me the updated line.

---

## Bruker

DOEN

---

## Assistent

Good. Now connect the button to a new function named `visHilsen10`.

You used the necessary HTML attribute in oppgave 8 to run `siHei()` when clicked. Add that same attribute, but make it call `visHilsen10()` instead. Show me the button line.

---

## Bruker

```xml
<button Lag hilsen onclick="visHilsen"></button>
```

---

## Assistent

The button text must stay between the tags, and a function call needs parentheses.

Use this structure:

```html
<button onclick="_____()">_____</button>
```

Fill the first blank with the function name `visHilsen10`, and the second with the visible text `Lag hilsen`. Rewrite the line.

---

## Bruker

```xml
<button onclick="visHilsen">Lag hilsen</button>
```

---

## Assistent

The visible text is correct.

Inside `onclick`, `visHilsen` currently only names the function. Add `()` immediately after it to **call** the function.

Make only that change. We can keep the shorter name `visHilsen` as long as the JavaScript function uses the exact same spelling.

---

## Bruker

ok

---

## Assistent

Now add an empty paragraph below the button where the result can appear.

Give it the unique ID `hilsen10`. Don’t change the JavaScript yet. Show me the paragraph line.

---

## Bruker

```xml
<input type="text" id="navn10">
<input type="number" id="alder10">
<button onclick="visHilsen()">Lag hilsen</button>
<input type="text" id="hilsen10">
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
    function visHilsen() {

    }
</script>
<p>se i console</p>
```

---

## Assistent

Your two inputs, button, and empty `visHilsen()` function are all correct.

One fix: `hilsen10` should display output, so it should be a paragraph—not another input field. An input is for the user to type into.

Change only the `hilsen10` element from an `<input>` to an empty `<p>` with the same ID.

---

## Bruker

doen

---

## Assistent

Good. Now `visHilsen()` must first find the name input.

Inside that function, create a `const` named `navnFelt` using `document.querySelector(...)`.

What selector should it use to find the input with `id="navn10"`? Answer with only the selector.

---

## Bruker

argument or vishilsen

---

## Assistent

Neither—those are JavaScript concepts.

A selector identifies an HTML element. You learned the rule in oppgave 8:

```text
# + elementets ID
```

The input’s ID is `navn10`, so its selector is `#navn10`.

What selector should we use? Include the `#`.

---

## Bruker

\#hilsen

---

## Assistent

`#hilsen` belongs to oppgave 8’s output paragraph.

Look at the current input:

```text
id="navn10"
```

Therefore its selector is:

```text
#navn10
```

That is the selector for the name input in oppgave 10. No code change yet—just remember that each selector matches the element’s exact ID.

---

## Bruker

```xml
<input type="text" id="navn10">
<input type="number" id="alder10">
<button onclick="visHilsen()">Lag hilsen</button>
<p id="hilsen10"></p>
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
    function visHilsen() {
        const navnfelt = document.querySelector("#hilsen10")
    }
</script>
<p>se i console</p>
```

---

## Assistent

Your `querySelector` pattern is correct, but `navnfelt` should point to the **name input**.

Currently it selects `#hilsen10`, which is the output paragraph. Change only the selector to match the name input’s ID: `#navn10`.

---

## Bruker

done
```xml
<h1>Oppgave 10</h1>
<input type="text" id="navn10">
<input type="number" id="alder10">
<button onclick="visHilsen()">Lag hilsen</button>
<p id="hilsen10"></p>
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
    function visHilsen() {
        const navnfelt = document.querySelector("#navn")
    }
</script>
<p>se i console</p>
```

---

## Assistent

Almost—you changed it to `#navn`, but that selects the old input from oppgave 8.

Your new input has:

```text
id="navn10"
```

So add `10` to the selector. Change only `#navn` to `#navn10`.

---

## Bruker

there

---

## Assistent

Good. Now repeat the same pattern for the age input.

Inside `visHilsen()`, add another `const`:

- Variable name: `alderfelt`
- Selector: `#alder10`

Write that line yourself and show me the function.

---

## Bruker

```javascript
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
```

---

## Assistent

Correct. Now find the output paragraph using the same pattern:

- Variable name: `hilsenfelt`
- Selector: `#hilsen10`

Add that as the third `const` inside `visHilsen()`.

---

## Bruker

```javascript
    }
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
        const hilsen = document.querySelector("#hilsen10")
```

---

## Assistent

Correct. You chose the shorter name `hilsen`, which is fine because it’s inside this function.

Now we need to read what the user typed into `navnfelt`. Which property gives us the current content of an input element? It starts with a dot.

---

## Bruker

ok

---

## Assistent

The property is `.value`, like in oppgave 8.

Create a `const` named `skrevetNavn10` and store `navnfelt.value` in it. Write that one line yourself.

---

## Bruker

```javascript
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
        const hilsen = document.querySelector("#hilsen10")
        const skrevetnavn10 = navnfelt.value
        const skrevetalder10 = alderfelt.value
        const skrevethilsen10 = hilsen.value
    }
```

---

## Assistent

The first two value lines are correct—you read both inputs.

The third is unnecessary:

```text
const skrevethilsen10 = hilsen.value
```

`hilsen` is a paragraph, not an input. We will **write** to it using `.textContent`, not read `.value` from it.

Delete only that third line.

---

## Bruker

done

---

## Assistent

Now call `lagHilsen` with two arguments.

The arguments must be the variables containing:

1. The typed name
2. The typed age

What are those two variable names, in that order? Answer without writing the function call yet.

---

## Bruker

what

---

## Assistent

Look at the left side of the two lines you just wrote:

```text
const skrevetnavn10 = ...
const skrevetalder10 = ...
```

So the variables are:

1. `skrevetnavn10`
2. `skrevetalder10`

Those will replace `"Kari"` and `17` when calling the function. Which one must go first?

---

## Bruker

isk

---

## Assistent

The name goes first because your function is defined as `(navn, alder)`.

Complete this call:

```javascript
lagHilsen(skrevetnavn10, _____)
```

The blank needs the variable containing the typed age. Which variable is that?

---

## Bruker

```javascript
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
        const hilsen = document.querySelector("#hilsen10")
        const skrevetnavn10 = navnfelt.value
        const skrevetalder10 = alderfelt.value
        lagHilsen(skrevetnavn10, skrevetalder10)
```

---

## Assistent

The function call is correct. It now creates the full greeting, but the returned result is still discarded.

To display it, assign that call’s result to the paragraph’s text. You already know:

- Paragraph variable: `hilsen`
- Property that changes displayed text: `.textContent`

Put `hilsen.textContent =` directly before your existing `lagHilsen(...)` call. Then test the button.

---

## Bruker

done

---

## Assistent

Test it:

- Enter `Kari` in the name field.
- Enter `17` in the age field.
- Click **Lag hilsen**.

It should display:

```text
Hei Kari! Du er 17 år gammel.
```

Does that exact sentence appear on the page?

---

## Bruker

index.html?vscode-livepreview=true:25 Adrian
index.html?vscode-livepreview=true:26 Uncaught TypeError: Assignment to constant variable.
&#x20;   at index.html?vscode-livepreview=true:26:14
(anonymous) @ index.html?vscode-livepreview=true:26
index.html?vscode-livepreview=true:34 0
index.html?vscode-livepreview=true:36 1
index.html?vscode-livepreview=true:46 string
index.html?vscode-livepreview=true:47 number
index.html?vscode-livepreview=true:48 undefined
index.html?vscode-livepreview=true:49 boolean
index.html?vscode-livepreview=true:58 Ingen melding enda
index.html?vscode-livepreview=true:65 javascript was here.
index.html?vscode-livepreview=true:103 Hei ola!
index.html?vscode-livepreview=true:124 Uncaught SyntaxError: Unexpected token '}' (at index.html?vscode-livepreview=true:124:9)
index.html?vscode-livepreview=true:110 Uncaught ReferenceError: visHilsen is not defined
&#x20;   at HTMLButtonElement.onclick (index.html?vscode-livepreview=true:110:35)
onclick @ index.html?vscode-livepreview=true:110
index.html?vscode-livepreview=true:110 Uncaught ReferenceError: visHilsen is not defined
&#x20;   at HTMLButtonElement.onclick (index.html?vscode-livepreview=true:110:35)
onclick @ index.html?vscode-livepreview=true:110

---

## Assistent

The main blocker is:

```text
Unexpected token '}'
```

That syntax error prevents the entire oppgave 10 script from loading, which is why `visHilsen is not defined` appears afterward.

Paste your complete oppgave 10 section, including `<script>`, `</script>`, and all closing braces. I’ll point out the mismatched brace without rewriting the solution.

The earlier `Assignment to constant variable` is a separate oppgave 1 issue we’ll fix afterward.

---

## Bruker

```xml
<h1>Oppgave 10</h1>
<input type="text" id="navn10">
<input type="number" id="alder10">
<button onclick="visHilsen()">Lag hilsen</button>
<p id="hilsen10"></p>
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
        const hilsen = document.querySelector("#hilsen10")
        const skrevetnavn10 = navnfelt.value
        const skrevetalder10 = alderfelt.value
        lagHilsen(skrevetnavn10, skrevetalder10)
        hilsen.textContent = 
    }
</script>
<p>se i console</p>
```

---

## Assistent

The closing brace is fine. The actual problem is this incomplete assignment:

```text
hilsen.textContent =
```

JavaScript expects a value after `=` but reaches `}` instead.

You currently have the required value on the line above:

```text
lagHilsen(skrevetnavn10, skrevetalder10)
```

Move that function call to directly after the `=`. Then delete the now-empty standalone call line. In other words, those two lines must become one assignment line.

Test again afterward.

---

## Bruker

what

---

## Assistent

You have two separate lines:

```text
lagHilsen(...)
hilsen.textContent =
```

The first line creates the greeting. The second line says where to display it, but it’s missing the greeting after `=`.

Do this:

1. Cut the entire `lagHilsen(...)` call from the first line.
2. Paste it immediately after `hilsen.textContent =`
3. Remove the empty line left behind.

The pattern should be:

```text
destination = returnedValue
```

You’re connecting the returned greeting to the paragraph.

---

## Bruker

```xml
<button onclick="visHilsen()">Lag hilsen</button>
<p id="hilsen10"></p>
<script>
    function lagHilsen(navn, alder){
       return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
    }
    function visHilsen() {
        const navnfelt = document.querySelector("#navn10")
        const alderfelt = document.querySelector("#alder10")
        const hilsen = document.querySelector("#hilsen10")
        const skrevetnavn10 = navnfelt.value
        const skrevetalder10 = alderfelt.value
        hilsen.textContent = lagHilsen(skrevetnavn10, skrevetalder10)
    }
```

---

## Assistent

Yes—that is correct. Oppgave 10 should now work.

Test the button again. If it displays the greeting, oppgave 10 is complete.

Then remove this old line from oppgave 1:

```text
navn = "Adrian";
```

You already created `navn` with `const`, so trying to assign it again causes the `Assignment to constant variable` error.

---

## Bruker

well it works

---

## Assistent

Nice—oppgave 10 is complete.

You now understand this chain:

`two inputs` → `.value` → two arguments → function parameters → `return` → `.textContent`

For oppgave 11, we can reuse the existing `melding` element from oppgave 4. Start by adding:

- Heading: `Oppgave 11`
- Button text: `Bytt farge`
- The button should call a function named `byttFarge()`

Write the heading and button yourself, then show me.

---

## Bruker

i am taking a break to tomorrow

---

## Assistent

Good stopping point. You completed oppgave 8, 9, and 10 today.

Tomorrow we’ll start with oppgave 11: changing CSS using JavaScript. Your next step will be creating the **Bytt farge** button.

Save your file before closing VS Code.

---

## Bruker

ok lets continue

---

## Assistent

Let’s continue with oppgave 11: changing CSS using JavaScript.

First step only:

- Add the heading `Oppgave 11`.
- Add a button displaying `Bytt farge`.
- Make the button call a function named `byttFarge()` when clicked.

Use oppgave 8’s button as your pattern, then paste what you write.

---

## Bruker

i dont think every task need a button because i saw my friends code wich the teacher helped him with and task 10 did not have button

---

## Assistent

You’re right that not every task requires a button.

For oppgave 10, the document only says to connect the function to two input fields. It doesn’t explicitly demand a button, although using one is a simple valid way to trigger the function.

Oppgave 11 **does explicitly require a button**:

> Lag en knapp Bytt farge. Når den trykkes skal JavaScript endre …

So keep your oppgave 10 button—it isn’t wrong or unnecessary functionality—and create the required **Bytt farge** button for oppgave 11.

---

## Bruker

```xml
<h1>Oppgave 11</h1>
<button onclick="byttfarge()">Bytt farge</button>
<script></script>
<p>Se over</p>
```

---

## Assistent

That’s correct. You chose the function name `byttfarge` with a lowercase `f`, so JavaScript must use that exact spelling everywhere.

Inside `<script>`, create an empty function named `byttfarge`. Don’t add CSS changes yet. Show me the function.

---

## Bruker

done

---

## Assistent

Good. We can reuse the `<h2>` from oppgave 4 as the message box. Its JavaScript variable was:

```text
melding
```

For CSS through JavaScript, the pattern is:

```text
element.style.cssProperty
```

The first required property is `backgroundColor`. Which element variable should come before `.style.backgroundColor`?

---

## Bruker

i am guessing melding so it knos what to change

---

## Assistent

Exactly. `melding` tells JavaScript which element to change.

So the left side becomes:

```text
melding.style.backgroundColor
```

Now assign it a color using `=` and a quoted CSS color such as `"lightblue"`. Choose any background color you want and show me the line.

---

## Bruker

where do i put this

---

## Assistent

Put it **inside the `byttfarge()` function**, between its `{` and `}`.

Why: code inside that function runs only when the button is clicked.

Structure:

```javascript
function byttfarge() {
    // Put the color-changing line here
}
```

Add your background-color line there and show me the function.

---

## Bruker

```xml
<script>
    function byttFarge() {
        melding.style.backgroundcolor = lightblue
    }
```

---

## Assistent

The line is in the correct place. There are three small case/syntax details to fix, one at a time.

First, your button calls `byttfarge()`, but your function is named `byttFarge()`. JavaScript treats those as different names.

Choose one spelling and make the button and function match exactly. Tell me which spelling you keep.

---

## Bruker

no i changed it to F

---

## Assistent

Good—then both should use `byttFarge()`.

Next, JavaScript writes the CSS property `background-color` as camelCase:

```text
backgroundColor
```

Change only the lowercase `c` in `backgroundcolor` to a capital `C`.

---

## Bruker

```xml
<button onclick="byttFarge()">Bytt farge</button>
<script>
    function byttFarge() {
        melding.style.backgroundColor = lightblue
    }
```

---

## Assistent

The function name and property are now correct.

`lightblue` is a text value—a CSS color name—so it needs quotation marks. Without them, JavaScript searches for a variable named `lightblue`.

Put quotation marks around the color, then test the button. Does the message background change?

---

## Bruker

doesnt what make it a fixed text

---

## Assistent

Yes—quotation marks make it fixed text, and that’s exactly what we need here.

CSS expects the color name as text:

```text
"lightblue"
```

Without quotation marks, JavaScript interprets `lightblue` as a variable and throws an error because that variable doesn’t exist.

So:

- `"lightblue"` → the CSS color light blue
- `lightblue` → a JavaScript variable named `lightblue`

Add the quotation marks and test it.

---

## Bruker

what should happen

---

## Assistent

When you click **Bytt farge**, the background behind the `<h2 id="melding">` text near oppgave 4 should turn light blue.

Only that message element should change—not the entire webpage.

If nothing changes, open the browser console and tell me the newest red error.

---

## Bruker

yeah it works

---

## Assistent

Great. Now add the second required CSS change inside the same function: the text color.

The JavaScript property is simply:

```text
color
```

Use the same pattern as `backgroundColor`, but choose a different readable color for the text. Add that line and tell me which color you chose.

---

## Bruker

what color fits with light blue

---

## Assistent

`"darkblue"` fits well with a light-blue background and gives good contrast.

Use `"darkblue"` as the text-color value.

---

## Bruker

ok next

---

## Assistent

The final required change is the font size.

CSS `font-size` becomes `fontSize` in JavaScript. Its value needs a unit, such as `"28px"`.

Add a third style line inside the function that changes `melding.style.fontSize` to `"28px"`, then test the button.

---

## Bruker

it works

---

## Assistent

Oppgave 11 is complete.

Now oppgave 12: count button clicks.

The counter must remember its value between clicks, so it needs to be declared **outside** the click function. It also changes from `0` to `1`, `2`, and so on, so it uses `let`.

Create the oppgave 12 heading and a `<script>` containing:

- A `let` variable named `antallKlikk`
- Starting value `0`

Don’t create the button or function yet. Show me what you write.

---

## Bruker

```xml
<h1>Oppgave 12</h1>
<script>
    let antallKlikk = "0"
</script>
```

---

## Assistent

Almost. A click count is a **number**, not text.

Quotation marks make `"0"` a string. Without quotation marks, `0` is a number that JavaScript can increase mathematically.

Remove the quotation marks around `0`. Then the variable is correct.

---

## Bruker

so i actually learned java now since i wrote it without help

---

## Assistent

You’ve learned a real piece of **JavaScript**: declaring a changeable number variable with `let`. Java and JavaScript are different languages.

The stronger sign of learning is that you can explain it:

- `let` because the click count will change.
- `0` without quotation marks because it’s a number.

That’s genuine progress—you’re starting to understand why the code is written that way.

---

## Bruker

ok

---

## Assistent

Next, add a button below the script:

- Visible text: `Tell klikk`
- On click, call a function named `tellKlikk()`

Use the same button pattern as oppgave 11, then show me the line.

---

## Bruker

ok

---

## Assistent

Now add an empty paragraph below the button to display the count. Give it the ID:

```text
klikkMelding
```

Show me that paragraph line.

---

## Bruker

done

---

## Assistent

Inside oppgave 12’s `<script>`, below the `let antallKlikk = 0` line, create an empty function named `tellKlikk`.

Make sure its spelling exactly matches the name used by the button. Show me the script section.

---

## Bruker

done

---

## Assistent

Now the function must increase the counter by one each time it runs.

JavaScript’s `++` means “increase this number by 1.” Inside `tellKlikk()`, add `++` immediately after the variable name `antallKlikk`.

Then tell me what value it has after the button is clicked three times.

---

## Bruker

like this


```xml
<h1>Oppgave 12</h1>
<script>
    let antallKlikk = 0
    function antallKlikk() {
        ++
    }
</script>
<button onclick="antallKlikk()">Tell klikk</button>
<p id="klikkmelding"></p>
<p>se i console</p>
```

---

## Assistent

You used `antallKlikk` for both the number and the function. JavaScript needs different names for different jobs:

- `antallKlikk` → the number
- `tellKlikk` → the function

First, rename the function to `tellKlikk` and make the button call `tellKlikk()`. Don’t change the `++` line yet. Show me the updated section.

---

## Bruker

z
```javascript
    let antallKlikk = 0
    function antallKlikk{
        ++
    }
</script>
<button onclick="antallKlikk()">Tell klikk</button>
<p id="klikkmelding"></p>
<p>se i console</p>
```

---

## Assistent

You haven’t renamed it yet, and the function also needs parentheses.

Change only the function opening:

- Replace the name `antallKlikk` with `tellKlikk`.
- Add empty parentheses `()` after `tellKlikk`.
- Keep the `{`.

Then change the button’s `onclick` to call the same name: `tellKlikk()`.

Do only those two name fixes first.

---

## Bruker

```xml
<script>
    let antallKlikk = 0
    function tellKlikk() {
        ++
    }
</script>
<button onclick="tellKlikk()">Tell klikk</button>
<p id="klikkmelding"></p>
<p>se i console</p>
```

---

## Assistent

The function and button now match correctly.

`++` cannot stand alone—it must know which number to increase. Put the counter variable’s name immediately before it:

```text
variableName++
```

Which variable should be increased when the button is clicked? Type only its name.

---

## Bruker

antallclick

---

## Assistent

The idea is right, but use the exact variable name you declared:

```text
antallKlikk
```

JavaScript spelling and capitalization must match exactly. Combine that name with `++` inside the function. What line do you get?

---

## Bruker

antallKlikk++

---

## Assistent

Correct. Add that line inside the function.

Next, the function must find the output paragraph. Its ID is `klikkmelding`.

What selector should `document.querySelector(...)` use to find it? Answer with only the selector.

---

## Bruker

klikkmelding

---

## Assistent

Almost. Because it is an ID, the selector needs `#`:

```text
#klikkmelding
```

Now create a `const` named `klikkElement` that uses `document.querySelector(...)` to find that selector. Write the line yourself.

---

## Bruker

```javascript
        const klikkelement = document.querySelector("#klikkmelding")
```

---

## Assistent

Correct.

Now display the changing count using this incomplete line:

```javascript
klikkelement.textContent = "Du har trykket " + _____ + " ganger.";
```

Which variable goes in the blank? It must contain the current number of clicks.

---

## Bruker

this is outside of function

---

## Assistent

It must go **inside** `tellKlikk()`. Otherwise it runs only once when the page loads.

Inside the function, the order should be:

1. Increase `antallKlikk`.
2. Find the paragraph.
3. Change the paragraph’s text.

Place the incomplete `.textContent` line after your `querySelector` line. Then fill the blank with the counter variable.

---

## Bruker

```javascript
        const klikkelement = document.querySelector("#klikkmelding")
```

---

## Assistent

Yes—keep that line inside `tellKlikk()`.

Directly below it, write:

```text
klikkelement.textContent = "Du har trykket " + [counter variable] + " ganger.";
```

Replace `[counter variable]` with the exact variable you increased using `++`. Show me the complete function when done.

---

## Bruker

```ini
        klikkelement.textContent = "Du har trykket " + antallKlikk + " antall ganger" 
```

---

## Assistent

Your JavaScript logic is correct. The text just differs slightly from the assignment.

It should display:

```text
Du har trykket 5 ganger.
```

So change `" antall ganger"` to `" ganger."` Then click the button several times and confirm the number increases.

---

## Bruker

it works

---

## Assistent

Oppgave 12 is complete.

Quick understanding check before oppgave 13:

Why must `antallKlikk` use `let`, while `klikkelement` can use `const`? Answer in your own words—a rough explanation is enough.

---

## Bruker

let is becaue it needs to let the number change

---

## Assistent

Correct. `let` allows the number stored in `antallKlikk` to change.

`klikkelement` can be `const` because it keeps referring to the same paragraph. We change the paragraph’s text, not which element the variable refers to.

Before oppgave 13, one small conflict: oppgave 3 already has `const elev = true`, but oppgave 13 needs `elev` to be an object. JavaScript won’t let you declare two global `const` variables with the same name.

In oppgave 3, rename the boolean variable from `elev` to `erElev`, including its `console.log`. This still matches the task better. Tell me when done.

---

## Bruker

\<!DOCTYPE html>
\<html lang="en">
\<head>
&#x20;   \<meta charset="UTF-8">
&#x20;   \<meta name="viewport" content="width=device-width, initial-scale=1.0">
&#x20;   \<title>Javascript 1\</title>
&#x20;   \<style>
&#x20;       body{
&#x20;           background-color: rgb(20, 20, 18); padding: 20px;
&#x20;       }
&#x20;       h1{
&#x20;           font-family: monospace; color: darkgreen;
&#x20;           color: rgb(176, 169, 169);
&#x20;       }
&#x20;       p{
&#x20;           color: rgb(176, 169, 169);
&#x20;       }
&#x20;   \</style>
\</head>
\<body>
&#x20;  &#x20;
&#x20;   \<h1>Oppgave 1\</h1>
&#x20;   \<script>
&#x20;       const navn = "Adrian";
&#x20;       console.log (navn);
&#x20;       navn = "Adrian";
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 2\</h1>
&#x20;   \<script>
&#x20;       let resultat = 0;
&#x20;       console.log (resultat);
&#x20;       resultat++;
&#x20;       console.log (resultat);
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 3\</h1>
&#x20;   \<script>
&#x20;       const alder = 17;
&#x20;       const erelev = true;
&#x20;       let tom;
&#x20;       console.log (typeof(navn));
&#x20;       console.log (typeof(alder));
&#x20;       console.log (typeof(tom));
&#x20;       console.log (typeof(erelev));
&#x20;   \</script>
&#x20;   \<style>\</style>
&#x20;   \<p>se console ->\</p>

&#x20;   \<h1>Oppgave 4\</h1>
&#x20;   \<h2 id="melding">Ingen melding enda\</h2>
&#x20;   \<script>
&#x20;       const melding = document.querySelector("#melding");
&#x20;       console.log (melding.innerHTML);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 5\</h1>
&#x20;   \<script>
&#x20;       melding.textContent = "javascript was here."
&#x20;       console.log (melding.textContent);
&#x20;   \</script>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 6\</h1>
&#x20;   \<script>
&#x20;       function visMelding() {
&#x20;           console.log ("knappen ble trykkket!");
&#x20;           melding.textContent="Du trykket på meg!";
&#x20;       }
&#x20;   \</script>
&#x20;   \<button onclick="visMelding()">Trykk på meg\</button>
&#x20;   \<p>se over og i console ->\</p>

&#x20;   \<h1>Oppgave 7\</h1>
&#x20;   \<p>Se funksjon i oppgave 6 (melding.textcontent)\</p>

&#x20;   \<h1>Oppgave 8\</h1>
&#x20;   \<input type="text" id="navn">&#x20;
&#x20;   \<button onclick="siHei()">Si hei\</button>
&#x20;   \<script>
&#x20;       function siHei() {
&#x20;           const inputFelt = document.querySelector("#navn");
&#x20;           const skrevetNavn = inputFelt.value;
&#x20;           console.log (inputFelt.value)
&#x20;           const hilsenelement = document.querySelector("#hilsen");
&#x20;           hilsenelement.textContent = "Hei " + skrevetNavn + "!"
&#x20;       }
&#x20;   \</script>
&#x20;   \<p id="hilsen">\</p>
&#x20;   \<p>se over og i console\</p>

&#x20;   \<h1>Oppgave 9\</h1>
&#x20;   \<script>
&#x20;       function lagHilsen(navn) {
&#x20;           return "Hei " + navn + "!";
&#x20;       }
&#x20;       const tekst = lagHilsen("ola")
&#x20;       console.log(tekst)
&#x20;   \</script>
&#x20;   \<p>se i console\</p>

&#x20;   \<h1>Oppgave 10\</h1>
&#x20;   \<input type="text" id="navn10">
&#x20;   \<input type="number" id="alder10">
&#x20;   \<button onclick="visHilsen()">Lag hilsen\</button>
&#x20;   \<p id="hilsen10">\</p>
&#x20;   \<script>
&#x20;       function lagHilsen(navn, alder){
&#x20;          return "Hei " + navn + "! " + "Du er " + alder + " år gammel.";
&#x20;       }
&#x20;       function visHilsen() {
&#x20;           const navnfelt = document.querySelector("#navn10")
&#x20;           const alderfelt = document.querySelector("#alder10")
&#x20;           const hilsen = document.querySelector("#hilsen10")
&#x20;           const skrevetnavn10 = navnfelt.value
&#x20;           const skrevetalder10 = alderfelt.value
&#x20;           hilsen.textContent = lagHilsen(skrevetnavn10, skrevetalder10)
&#x20;       }
&#x20;   \</script>
&#x20;   \<p>se i console\</p>

&#x20;   \<h1>Oppgave 11\</h1>
&#x20;   \<button onclick="byttFarge()">Bytt farge\</button>
&#x20;   \<script>
&#x20;       function byttFarge() {
&#x20;           melding.style.backgroundColor = "lightblue"
&#x20;           melding.style.color = "darkblue"
&#x20;           melding.style.fontSize = "28px"
&#x20;       }
&#x20;   \</script>
&#x20;   \<p>Se på oppgave 4\</p>

&#x20;   \<h1>Oppgave 12\</h1>
&#x20;   \<script>
&#x20;       let antallKlikk = 0
&#x20;       function tellKlikk() {
&#x20;           antallKlikk++
&#x20;           const klikkelement = document.querySelector("#klikkmelding")
&#x20;           klikkelement.textContent = "Du har trykket " + antallKlikk + " ganger"&#x20;
&#x20;       }
&#x20;   \</script>
&#x20;   \<button onclick="tellKlikk()">Tell klikk\</button>
&#x20;   \<p id="klikkmelding">\</p>
&#x20;   \<p>se i console\</p>
\</body>
\</html>

---

## Assistent

Your rename works. I’d spell it `erElev` with a capital `E` for readability, but `erelev` is still valid if used consistently.

One old error remains in oppgave 1:

```javascript
navn = "Adrian";
```

Delete that second assignment. `navn` is already created as a `const`, so assigning to it again causes the red `Assignment to constant variable` error.

Make only that fix first. Then we’ll start the object in oppgave 13.

---

## Bruker

done

---

## Assistent

Now oppgave 13: an **object** groups related information into one value.

For example, instead of four unrelated variables, one `elev` object will contain four properties:

- `navn`
- `alder`
- `klasse`
- `erElev`

Start with the heading and an empty object inside `<script>`:

- Variable name: `elev`
- Use `const`
- An object uses `{ }`

Write that part yourself and show me.

---

## Bruker

i dont know what object is

---

## Assistent

An object is one container holding several related pieces of information.

Think of a student card:

```text
elev
├── navn: "Kari"
├── alder: 17
├── klasse: "2ITA"
└── erElev: true
```

Each labeled piece is called a **property**.

Unrelated JavaScript example:

```javascript
const bil = {
    merke: "Volvo",
    år: 2020
};
```

Here:

- `bil` is the object.
- `merke` and `år` are properties.
- `"Volvo"` and `2020` are their values.

In `bil.merke`, which part is the object’s name: `bil` or `merke`?

---

## Bruker

ok done

---

## Assistent

Paste only your oppgave 13 section so I can see what you created.

---

## Bruker

is this only inside console or does the page change
```xml
<h1>Oppgave 13</h1>
<script>
    const elev{
        
    }
</script>
```

---

## Assistent

Oppgave 13 only writes information to the **console**. It does not need to change the webpage.

Your object is almost started correctly, but variable assignment requires `=`:

```text
const elev = {
    
}
```

Add the equals sign between `elev` and `{`. Then we’ll add one property at a time.

---

## Bruker

done

---

## Assistent

Inside an object, a property uses:

```text
propertyName: value
```

Add the first property:

- Property name: `navn`
- Value: your name as text

Remember that text needs quotation marks. Show me the property line you write.

---

## Bruker

done

---

## Assistent

Now add a comma after the `navn` property, then add:

- Property name: `alder`
- Value: your age as a number, without quotation marks

Show me the object after adding it.

---

## Bruker

done

---

## Assistent

Add the third property:

- Property name: `klasse`
- Value: your class as quoted text, for example `"2ITA"`

Remember the comma separating it from the previous property. Show me the object afterward.

---

## Bruker

done

---

## Assistent

Add the final property:

- Property name: `erElev`
- Value: `true` without quotation marks, because it’s a boolean

Then paste the complete `elev` object so we can check it.

---

## Bruker

```javascript
    const elev = {
        navn: "Adrian", alder: 17, klasse: "2ITA", erElev: true
    }
```

---

## Assistent

Correct—that is a valid object with four properties. Writing them on one line works, though one property per line is usually easier to read.

Now write the **entire object** to the console. Which variable should go inside `console.log(...)`? Type only the variable name.

---

## Bruker

elev

---

## Assistent

Correct. Add `console.log(elev)` below the object.

Next, the assignment asks you to print only the student’s name. A property is accessed with:

```text
object.property
```

Using your object and its `navn` property, what expression gets only the name?

---

## Bruker

where still on 13

---

## Assistent

Yes, still inside oppgave 13’s `<script>`.

Put the `console.log` lines **after the object’s closing `}`**, but before `</script>`:

```text
const elev = {
    properties here
}

console.log goes here
another console.log goes here
```

The object must be fully created before you print it. Add the first log for the entire `elev` object.

---

## Bruker

adrian

---

## Assistent

`Adrian` is the value you expect to see in the console.

But the JavaScript expression that retrieves it is:

```text
elev.navn
```

- `elev` identifies the object.
- `.navn` selects its name property.

Put `elev.navn` inside the second `console.log(...)`. Then oppgave 13 is complete.

---

## Bruker

```xml
<script>
    const elev = {
        navn: "Adrian", alder: 17, klasse: "2ITA", erElev: true
    }
    Object.navn
    console.log(elev.navn);
</script>
```

---

## Assistent

`console.log(elev.navn)` is correct.

Delete this unnecessary line:

```text
Object.navn
```

`Object` with a capital `O` is a built-in JavaScript object, not your student.

You’re also missing the log for the complete object. Add `console.log(...)` above the name log, using only `elev` inside the parentheses. Then oppgave 13 is complete.

---

## Bruker

done

---

## Assistent

Oppgave 13 is complete.

Oppgave 14 adds a **method** to the same `elev` object. A method is a function stored inside an object.

First step:

- Add a comma after `erElev: true`.
- Still inside the object, create an empty method named `presenter`.
- A method has parentheses `()` and braces `{}`.

Don’t add its console message yet. Show me the updated object.

---

## Bruker

{navn: 'Adrian', alder: 17, klasse: '2ITA', erElev: true}
index.html?vscode-livepreview=true:156 Adrian

---

## Assistent

That console output confirms oppgave 13 works:

- First line: the complete object
- Second line: only `Adrian`

Now edit the object in your code. After `erElev: true`, add a comma. On the next line, create an empty method named `presenter` using this shape:

```text
methodName() {
}
```

Replace `methodName` with `presenter`, then paste the updated object.

---

## Bruker

no its like that in console

---

## Assistent

Yes—that is exactly how it should appear in the console. Oppgave 13 is working correctly.

The console shows:

- `{navn: 'Adrian', ...}` because you logged `elev`.
- `Adrian` because you logged `elev.navn`.

Now return to the editor. We’ll modify the `elev` object itself for oppgave 14. Paste the object’s code from your editor when you’re ready.

---

## Bruker

ok

---

## Assistent

Inside the `elev` object:

1. Add a comma after `erElev: true`.
2. Add an empty method named `presenter`.

The method follows this pattern:

```text
presenter() {
}
```

Paste the updated object afterward.

---

## Bruker

whats a method

---

## Assistent

A **method** is a function that belongs to an object.

Think of an object as having:

- **Properties**: information it has
- **Methods**: actions it can perform

Example:

```javascript
const hund = {
    navn: "Luna",
    bjeff() {
        console.log("Voff!");
    }
};
```

Here:

- `navn` is a property.
- `bjeff()` is a method.
- `hund.bjeff()` runs the method.

For your student:

- `elev.navn` gets information.
- `elev.presenter()` performs an action: presenting the student.

Is `alder` a property or a method?

---

## Bruker

what

---

## Assistent

Simpler:

- A **property** stores a value: `alder: 17`
- A **method** runs code: `presenter()`

So `alder` is a property because it stores `17`.

`presenter()` will be a method because it will run code that prints a sentence. It’s basically a function placed inside the `elev` object. No coding yet—just remember: **property = information, method = action**.

---

## Bruker

what do i write

---

## Assistent

Inside the `elev` object, add a comma after `erElev: true`, then write:

```javascript
presenter() {
    
}
```

This only creates the empty method. We’ll work out what goes inside it next.

---

## Bruker

ok

---

## Assistent

Now learn `this`.

Inside an object’s method, `this` means “this object.” Therefore:

```text
this.navn
```

means the `navn` property belonging to the current `elev` object.

Inside `presenter()`, add a `console.log` that prints only `this.navn`. Don’t build the full sentence yet. Then show me the method.

---

## Bruker

```javascript
   const elev = {
        navn: "Adrian", alder: 17, klasse: "2ITA", erElev: true,
        presenterer() {
            this.navn
            console.log(this.navn)
        }
    }7
```

---

## Assistent

You’re close. Fix three small things:

1. The assignment requires the method name `presenter`, not `presenterer`.
2. Delete the standalone `this.navn` line—it does nothing by itself.
3. Delete the accidental `7` after the object’s closing brace; it will cause an error.

Keep `console.log(this.navn)` inside the method. Then paste the cleaned object.

---

## Bruker

```xml
<h1>Oppgave 13</h1>
<script>
    const elev = {
        navn: "Adrian", alder: 17, klasse: "2ITA", erElev: true,
        presenter() {
            console.log(this.navn)
        }
    }
```

---

## Assistent

The method itself is correct.

A method doesn’t run merely because it exists. You must call it after the object’s closing `}`.

The pattern is:

```text
objectName.methodName()
```

Using your object `elev` and method `presenter`, what call do you write?

---

## Bruker

elev.presenter()

---

## Assistent

Correct. Add `elev.presenter()` below the object and test it. The console should print `Adrian`.

Now we need the complete sentence:

```text
Jeg heter Adrian og går i 2ITA.
```

You already know `this.navn` gives `Adrian`. Which expression gives the student’s class? Use `this`.

---

## Bruker

i accidently added it to 13 could you just fix it quick     \<h1>Oppgave 13\</h1>
&#x20;   \<script>
&#x20;       const elev = {
&#x20;           navn: "Adrian", alder: 17, klasse: "2ITA", erElev: true,
&#x20;           presenter() {
&#x20;               console.log(this.navn)
&#x20;           }
&#x20;       }
&#x20;       elev.presenter()
&#x20;       console.log(elev)
&#x20;       console.log(elev.navn);
&#x20;   \</script>
&#x20;   \<p>se i console ->\</p>

&#x20;   \<h1>Oppgave 14\</h1>
&#x20;   \<script>

&#x20;   \</script>
\</body>
\</html>

---

## Assistent

Yes. To keep oppgave 13 and 14 separate, remove `presenter()` and `elev.presenter()` from oppgave 13.

Keep oppgave 13 as the object plus its two `console.log` calls. Then put this idea in oppgave 14:

```javascript
elev.presenter = function () {
    console.log("Jeg heter " + this.navn + " og går i " + this.klasse + ".");
};

elev.presenter();
```

This adds the `presenter` method to the existing `elev` object, then calls it.

The console should show:

```text
Jeg heter Adrian og går i 2ITA.
```

This is valid even though `elev` uses `const`: the variable still refers to the same object; you’re only adding something inside that object.

---

## Bruker

you do that but dont add what i ahevnt done yet

---

## Assistent

Jeg flytter bare det du allerede har laget: `presenter`-metoden og kallingen til oppgave 14. Jeg legger ikke til den ferdige presentasjonsteksten eller noe nytt. Først trenger jeg skrivetilgang til HTML-filen i Git-mappen.

---

## Bruker

no i gave you the code i can jyst copy paste

---

## Assistent

Sorry—I misunderstood. I edited the actual file instead of giving you a snippet to copy.

The file now has only your existing work moved:

- Oppgave 13 contains the object and its two logs.
- Oppgave 14 contains the existing `presenter` method that logs `this.navn`, plus its call.
- I did not add the finished presentation sentence.

From now on, I’ll only give you guidance or copyable snippets unless you explicitly ask me to edit the file.

---

## Bruker

no

---

## Bruker

no that worked too :)

---

## Assistent

Great 😄 Oppgave 13 and 14 are now separated correctly.

We’re still midway through oppgave 14: `presenter()` currently prints only the name. Next, we’ll teach it to produce:

```text
Jeg heter Adrian og går i 2ITA.
```

We’ll continue one small piece at a time.

---

## Bruker

ok

---

## Assistent

Inside `presenter()`, you already use `this.navn` for the name.

The object also has the property `klasse`. What expression retrieves that property using `this`? Type only the expression.

---

## Bruker

```xml
<script>
    elev.presenter = function() {
        console.log(this.navn)
        console.log(this.klasse)
    }
    elev.presenter()
    klasse.presenter()
```

---

## Assistent

`console.log(this.klasse)` is correct—it accesses the class.

Delete this line:

```text
klasse.presenter()
```

`klasse` is only a property value (`"2ITA"`), not an object with a method. The method belongs to `elev`, so `elev.presenter()` is the only call needed.

After deleting it, the console should print `Adrian` and `2ITA` on separate lines. Then we’ll combine them into one sentence.

---

## Bruker

ok

---

## Assistent

Now replace the two separate logs with one incomplete sentence:

```javascript
console.log("Jeg heter " + this.navn + _____ + this.klasse + ".");
```

The blank needs fixed text between the name and class. What quoted text should go there so the result becomes:

```text
Jeg heter Adrian og går i 2ITA.
```

---

## Bruker

ok done but i feel like giving ao muvh code is a little cheating

---

## Assistent

You’re right—that scaffold gave away too much of the structure.

From now on, I’ll only:

- Explain the concept.
- Point out errors in code you write.
- Ask guiding questions.
- Avoid partial solution lines unless you explicitly request one.

For now, run `elev.presenter()`. If the console shows `Jeg heter Adrian og går i 2ITA.`, oppgave 14 is complete. Does it?

---

## Bruker

yes

---

## Assistent

Oppgave 14 is complete.

Now oppgave 15 combines earlier skills into an elevkort. We’ll build it in small parts, but you’ll decide and write the code.

First, no coding: according to the assignment, what three pieces of information must the user enter?

---

## Bruker

give me the whole task

---

## Assistent

## 15. Sluttoppgave – elevkort

Lag et lite elevkort på nettsiden.

Brukeren skal kunne skrive inn:

- navn
- alder
- klasse

Når brukeren trykker **Opprett elev**, skal JavaScript:

- hente verdiene fra input-feltene
- opprette et elev-objekt med verdiene
- bruke en metode i objektet til å lage en presentasjon
- vise presentasjonen på nettsiden
- endre CSS på elevkortet
- skrive det ferdige elev-objektet til konsollen

Resultatet kan for eksempel være:

```text
-----------------------------
          ELEVKORT

Navn: Kari Hansen
Alder: 17
Klasse: 2ITA

Kari går i 2ITA og er 17 år.
-----------------------------
```

Du skal sette sammen ting du allerede har brukt:

```text
input
↓
DOM
↓
.value
↓
funksjon
↓
objekt
↓
egenskaper + metode
↓
DOM
↓
resultat på nettsiden
```

Det er hele oppgave 15. Vi kan bygge den stegvis uten at jeg gir deg koden.

---

## Bruker

ok

---

## Assistent

First step: create the HTML inputs only.

Add:

- The heading `Oppgave 15`
- A text input for name
- A number input for age
- A text input for class

Choose unique IDs so they don’t conflict with earlier tasks. A sensible naming pattern is `navn15`, `alder15`, and `klasse15`.

Don’t add JavaScript or a button yet. Paste what you write.

---

## Bruker

done

---

## Assistent

Next, add the required **Opprett elev** button.

Make it call a function named `opprettElev()` when clicked. Don’t create the function yet. Paste the button line when done.

---

## Bruker

```xml
<h1>Oppgave 15</h1>
<input type="text" id="navn20">
<input type="number" id="alder20">
<input type="text" id="klasse20">
<button onclick="opprettElev()"> Opprett elev</button>
<script>
    function opprettElev() {
        
    }
</script>
```

---

## Assistent

That setup is correct. The IDs ending in `20` are fine as long as you use those exact IDs in JavaScript.

Now the page needs an empty container where the finished student card will appear. A `<div>` is suitable because it can hold several lines and be styled as a box.

Add an empty `div` with the ID `elevkort` below the button. Don’t change the function yet. Show me that line.

---

## Bruker

done

---

## Assistent

Inside `opprettElev()`, first find the name input with `document.querySelector`.

Your name input has `id="navn20"`. What selector must you use? Answer with only the selector.

---

## Bruker

\#navn20

---

## Assistent

Correct.

Inside `opprettElev()`, create four `const` references:

- `navnfelt20` finds `#navn20`
- `alderfelt20` finds `#alder20`
- `klassefelt20` finds `#klasse20`
- `elevkort` finds `#elevkort`

Use `document.querySelector` for each. Paste only the function when done.

---

## Bruker

```xml
<input type="text" id="navn20">
<input type="number" id="alder20">
<input type="text" id="klasse20">
<button onclick="opprettElev()"> Opprett elev</button>
<div id="elevkort"></div>
<script>
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
    }
</script>
```

---

## Assistent

Correct. Now read the three user-entered values with `.value`.

Create three new `const` variables inside the function:

- `skrevetNavn20`
- `skrevetAlder20`
- `skrevetKlasse20`

Each should receive the `.value` from its matching input element. Do not read a value from `elevkort` because it is an output container. Paste the three new lines.

---

## Bruker

```javascript
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
    }
```

---

## Assistent

Correct.

Now create the student object **inside** `opprettElev()`. Use the variable name `nyElev` so it’s clearly the newly created student.

Give it these three properties:

- `navn` gets the value from `skrevetnavn20`
- `alder` gets the value from `skrevetalder20`
- `klasse` gets the value from `skrevetklasse20`

Don’t add the method yet. Build the object yourself and paste only that part.

---

## Bruker

i dont remember how

---

## Assistent

An object uses curly braces, with each property written as:

```text
propertyName: value
```

Unrelated example:

```javascript
const nyttProdukt = {
    navn: skrevetProduktnavn,
    pris: skrevetPris
};
```

For your student:

- Object variable: `nyElev`
- Properties: `navn`, `alder`, `klasse`
- Values: the three variables you just created

Use the same pattern and try building it. Commas separate the properties.

---

## Bruker

done

---

## Assistent

Paste only your `nyElev` object so I can check it before we add its method.

---

## Bruker

```javascript
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20

        }
    }
```

---

## Assistent

The object is correct.

Now add a method inside `nyElev`:

1. Add a comma after the `klasse` property.
2. Add an empty method named `presenter()` below it.

Don’t create the sentence yet. Paste the object with the empty method.

---

## Bruker

```javascript
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20,
            presenter()
        }
```

---

## Assistent

Almost. `presenter()` currently has parentheses but no method body.

A method needs curly braces after its parentheses:

```text
presenter() {
    
}
```

Add the opening and closing braces. Make sure the object itself still has its separate closing `}` afterward. Then paste just the bottom of the object.

---

## Bruker

done

---

## Assistent

The method must create this sentence:

```text
Kari går i 2ITA og er 17 år.
```

Because the information belongs to `nyElev`, the method should access it through `this`.

What three `this` expressions retrieve the name, class, and age? List them in that order.

---

## Bruker

```xml
<h1>Oppgave 15</h1>
<input type="text" id="navn20">
<input type="number" id="alder20">
<input type="text" id="klasse20">
<button onclick="opprettElev()"> Opprett elev</button>
<div id="elevkort"></div>
<script>
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20,
            presenter() {
                console.log(this.navn + " går i " + this.klasse + " og er " + this.alder + "år.")
            }
        }
    }
</script>
```

---

## Assistent

Your sentence construction is almost correct, and you used all three `this` properties properly.

Two fixes:

1. The method needs to **return** the sentence so the webpage can use it. Replace the surrounding `console.log(...)` with `return`.
2. Add a space before `år`, otherwise it displays `17år`.

After the change, the method should return the text rather than print it. Paste only the updated method.

---

## Bruker

presenter() {
                    return console.log(this.navn + " går i " + this.klasse + " og er " + this.alder + " år.")
                }

---

## Assistent

Don’t combine `return` and `console.log`.

`console.log(...)` prints the sentence but returns `undefined`. Then your method would return that `undefined`.

For this method, use only `return`:

- Remove `console.log(`.
- Remove its matching final `)`.
- Keep the text-building expression directly after `return`.

The method should return the sentence without logging it. Try that change.

---

## Bruker

```kotlin
                return this.navn + " går i " + this.klasse + " og er " + this.alder + " år."
```

---

## Assistent

Correct—the method now returns the presentation.

Next, call that method after the `nyElev` object has been created. The pattern is:

```text
objectName.methodName()
```

What expression calls the `presenter` method belonging to `nyElev`? Type only the expression.

---

## Bruker

where

---

## Assistent

Put the method call:

- After the `nyElev` object’s closing `}`
- But still inside the `opprettElev()` function

Structure:

```text
function opprettElev() {
    inputs and values

    const nyElev = {
        properties and method
    }

    method call goes here
}
```

The object must exist before its method can be called. What expression calls `presenter()` on `nyElev`?

---

## Bruker

```
        nyElev.presenter()
```

---

## Assistent

Correct. That calls the method, but its returned sentence is currently discarded.

Store the returned sentence in a new constant named `presentasjon`. Put `const presentasjon =` before your existing method call.

This gives you a variable containing:

```text
Adrian går i 2ITA og er 17 år.
```

Make that change.

---

## Bruker

```javascript
        const presentasjon = nyElev.presenter()
```

---

## Assistent

Correct.

Now display `presentasjon` inside the `elevkort` div. Which property have you used in earlier tasks to change an element’s visible text? Answer with only the property name.

---

## Bruker

idk

---

## Assistent

The property is:

```text
.textContent
```

You used it in oppgave 8 and 12.

Now combine:

- Output element: `elevkort`
- Text property: `.textContent`
- Value to display: `presentasjon`

Write the assignment yourself inside `opprettElev()`, after creating `presentasjon`.

---

## Bruker

```xml
<button onclick="opprettElev()"> Opprett elev</button>
<div id="elevkort"></div>
<script>
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20,
            presenter() {
                return this.navn + " går i " + this.klasse + " og er " + this.alder + " år."
            }
        }
        const presentasjon = nyElev.presenter()
        elevkort.textContent.value
    }
```

---

## Assistent

`elevkort` is not an input, so `.value` doesn’t belong after `.textContent`.

You need an assignment:

- Left side: the card’s text property
- `=`
- Right side: the `presentasjon` variable

Remove `.value`, then assign `presentasjon` to `elevkort.textContent`. This follows the same `destination = value` pattern as oppgave 10.

---

## Bruker

```
        elevkort.textContent.presentasjon
```

---

## Assistent

You’re using a dot where an equals sign is needed.

In:

```text
elevkort.textContent.presentasjon
```

keep the first dot because `textContent` is a property of `elevkort`.

Replace the **second dot**—the one before `presentasjon`—with `=`. That assigns the returned presentation to the card’s text. Then test the button.

---

## Bruker

it works but the color is black an the backgound is black

---

## Assistent

That happens because the page background is dark while the card’s default text color is black.

Use what you learned in oppgave 11. Inside `opprettElev()`, after setting `textContent`, add the same two style changes—but target `elevkort` instead of `melding`:

- Background color: `"lightblue"`
- Text color: `"darkblue"`

Try writing those two style lines yourself. The relevant properties are `backgroundColor` and `color`.

---

## Bruker

```xml
<h1>Oppgave 15</h1>
<input type="text" id="navn20">
<input type="number" id="alder20">
<input type="text" id="klasse20">
<button onclick="opprettElev()"> Opprett elev</button>
<div id="elevkort"></div>
<script>
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20,
            presenter() {
                return this.navn + " går i " + this.klasse + " og er " + this.alder + " år."
            }
        }
        const presentasjon = nyElev.presenter()
        elevkort.textContent = presentasjon
    }
    function byttFarge() {
        melding.style.backgroundColor = "lightblue"
        melding.style.color = "darkblue"
        melding.style.fontSize = "28px"
    }
</script>
```

---

## Assistent

You copied the oppgave 11 function, but it still targets `melding`, and nothing calls it here.

For oppgave 15, CSS should change when **Opprett elev** runs.

Do this:

1. Delete the new `byttFarge()` function from oppgave 15.
2. Inside `opprettElev()`, directly after `elevkort.textContent = presentasjon`, add style changes targeting `elevkort`.
3. Use `backgroundColor` and `color`, with quoted color values.

The key difference is: target the student card (`elevkort`), not the old message (`melding`).

---

## Bruker

it wokrs

---

## Assistent

Great. Two requirements remain.

First, the assignment says to print the finished student object to the console. Which variable contains that object: `elevkort`, `presentasjon`, or `nyElev`?

---

## Bruker

elevkort

---

## Assistent

`elevkort` is the HTML element where the result appears.

The actual student object—with `navn`, `alder`, `klasse`, and `presenter()`—is `nyElev`.

Add a `console.log` for `nyElev` inside `opprettElev()`. Then clicking **Opprett elev** will print the finished object.

---

## Bruker

```javascript
    function opprettElev() {
        const navnfelt20 = document.querySelector("#navn20")
        const alderfelt20 = document.querySelector("#alder20")
        const klassefelt20 = document.querySelector("#klasse20")
        const elevkort = document.querySelector("#elevkort")
        const skrevetnavn20 = navnfelt20.value
        const skrevetalder20 = alderfelt20.value
        const skrevetklasse20 = klassefelt20.value
        const nyElev = {
            navn: skrevetnavn20,
            alder: skrevetalder20,
            klasse: skrevetklasse20,
            presenter() {
                return this.navn + " går i " + this.klasse + " og er " + this.alder + " år."
            }
        }
        const presentasjon = nyElev.presenter()
        elevkort.textContent = presentasjon
        elevkort.style.backgroundColor = "lightblue"
        elevkort.style.color = "darkblue"
        elevkort.style.fontSize = "28px"
        console.log(elevkort)
    }
</script>
```

---

## Assistent

Everything else is working, but the last line logs the HTML `<div>`, not the student object.

Change only the word inside `console.log(...)`:

- Current: `elevkort`
- Required object: `nyElev`

Afterward, the console should show an object containing the name, age, class, and method.

---

## Bruker

well it looks like a code

---

## Assistent

That’s normal. Browser consoles display JavaScript objects in a code-like format, for example:

```text
{navn: "Adrian", alder: "17", klasse: "2ITA", presenter: ƒ}
```

That means you successfully logged the object.

If it instead shows something beginning with `<div id="elevkort">`, you’re still logging the HTML element. Which of those two forms do you see?

---

## Bruker

{navn: 'kari', alder: '17', klasse: '2ita', presenter: ƒ} this

---

## Assistent

That is correct. `presenter: ƒ` means the object contains a function—the method you created.

Oppgave 15 now satisfies the required parts:

- Reads three input values
- Creates a student object
- Uses properties
- Uses a `presenter()` method
- Returns and displays the presentation
- Changes the card’s CSS
- Logs the completed object

The detailed card layout in the assignment is introduced as an example, so your styled card with the presentation is a valid simpler result. Oppgave 15 is complete.

---

## Bruker

lets go

---

## Assistent

Let’s go! You completed oppgave 8–15 and wrote the important parts yourself.

You’ve now used:

- DOM and `querySelector`
- `.value`, `.textContent`, and `.style`
- Functions, parameters, arguments, and `return`
- `let`, `const`, and click counting
- Objects, properties, methods, and `this`

Save the file and test every button once. You’re done.

---

## Bruker

# Files pasted by the user:

## "<!DOCTYPE html> <html lang=\"en\"> <head> <meta charset=\"UTF-8\"> <meta name=\"view…": C:\Users\adrse\.codex/attachments/56c0d109-b2c2-4b9b-a38b-2f2530e48938/pasted-text.txt

## My request:
now add a read me heres the code

---

## Assistent

Jeg lager en kort README som beskriver oppgavesettet, hva du har lært, og hvordan siden kjøres. Først leser jeg den ferdige koden og sjekker prosjektmappen.

---

## Assistent

Koden er gjennomgått. Jeg lager README-en på norsk i samme Git-prosjekt, uten å endre `index.html`.

---

## Assistent

Added `README.md` to:

`C:\Users\adrse\git\javascript\README.md`

It includes the project overview, concepts learned, all 15 tasks, instructions for running the page, and a description of the final student-card task. I did not modify `index.html`.

---

## Bruker

also the things i did that wasnt a task

---

## Assistent

Jeg legger til en egen seksjon om ekstraarbeidet ditt: det mørke designet, tydelig navigasjon/veiledning, riktige input-typer, testing med konsollen og prosjektets README.

---

## Assistent

Updated the README with an **Ekstraarbeid** section covering your:

- Custom dark design and colors
- Monospace headings
- Helper text
- Number input for ages
- Unique element IDs
- Live Preview and console testing
- Debugging work
- README documentation

---

## Bruker

je endret bakgrunnen til svart fordi jeg sitter i mørket så hvit bakgrunn er helt forferdelig

---

## Assistent

Det er en god og konkret begrunnelse. Jeg endrer README-en så den forklarer at mørkt tema ble valgt for bedre komfort og mindre blending i et mørkt rom.

---

## Assistent

README-en forklarer nå hvorfor du valgte mørkt tema: mindre blending og mer behagelig arbeid når du sitter i et mørkt rom. Det viser at designvalget ditt hadde en praktisk grunn, ikke bare var pynt.

---

## Bruker

this is great now i juat have to push and commit which i know how to do

---

## Assistent

Perfect. Before committing, run:

```bash
git status
git diff
```

Confirm that `index.html` and `README.md` are the intended changes, then commit and push using your usual workflow. Nice work—you completed the code and understood the concepts behind it.

---

## Bruker

jeg trenger hele denne chatten

---

## Assistent

Vil du ha hele chatten som en delbar lenke, eller som en Markdown-/tekstfil?

---

## Bruker

md funke

