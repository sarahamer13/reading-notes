### *What is a ‘Controlled Component’?* ###

- An input form element whose value is controlled by React in this way is called a “controlled component"

### *Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why* ###

- We should first store the user responses from the form before we update state because if state attempt to update with the user responses before it stores, it's going to break the site.

### *How do we target what the user is entering if we have an event handler on an input field?* ###

- You would create an event.target.value.


### *Why would we use a ternary operator?* ###

- It makes the code simpler to read and it makes it cleaner

### *Rewrite the following statement using a ternary statement:* ###

- x===y ?
console.log(true): console.log(false)

(References:https://legacy.reactjs.org/docs/forms.html,https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff )