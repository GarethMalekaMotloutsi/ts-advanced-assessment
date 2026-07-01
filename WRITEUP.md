# Assessment 2 Write-up

## Question 1

Generic constraints help make sure I only use keys that actually exist in an object. This helped me avoid mistakes while working through the exercises because TypeScript picked up errors before I even ran the code. Using `any` doesn't give you that protection.

## Question 2

I'd use a mapped type if I wanted to change every property in a type, like making everything readonly or allowing null values. I'd use `Pick` when I only need a few properties from an existing type instead of creating a new one myself.

## Question 3

`unknown` is safer than `any` because I have to check what the value is before I can use it. With `any`, TypeScript basically stops checking. A type guard is also safer than casting because it checks the value first instead of just assuming it's the correct type.

## Question 4

The `never` check makes sure I haven't forgotten to handle any actions in the reducer. If another action gets added later and I don't update the switch statement, TypeScript will let me know, which helps prevent bugs.