# Feedback App with Svelte

In this project we will learn the basics of the Svelte  framework.

## Create New App

```
npx degit sveltejs/template feedback-app
```
## Install the dependencies

```
npm i
```

## Build the project on dev mode

```
npm run dev
```

## Clean the starter
- src/App.svelte
- src/main.js
## Create a feedback variable as an array of objects like:
```
let feedback = [
  {
    id: 1,
    rating: 5,
    text: "rating text 1"
  },
  {
    id: 2,
    rating: 6,
    text: "rating text 2"
  },
  {
    id: 3,
    rating: 7,
    text: "rating text 3"
  },
]
```
## Create a feedbackList and feedbackItem components 
![](/assets/img1.png)

## Pass the feedback variable to the FeedbackList component
- App
```
<main>
	<FeedbackList feedback="{feedback}" /> 
	<!-- 
		Equivalent to: 
		<FeedbackList {feedback} /> 
	 -->
	
</main>
```
- FeedbackList
```
<script>
  export let feedback = []
  console.log(feedback)
</script>
```