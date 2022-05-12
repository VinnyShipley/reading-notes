# React and Forms

## React DOCS

1. **What is a ‘Controlled Component’?** A controlled component is an element whose value is controlled by React.

2. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them?**

3. **How do we target what the user is entering if we have an event handler on an input field?** If the event handler is ```handleChange(event) {this.setState({value: event.target.value});}``` then to target it, you would code ```<select value={this.state.value} onChange={this.handleChange}>```

## Ternaries

1. **Why would we use a ternary operator?** Ternaries are a shorthand of true or false what if statements.

2. **The rewritten statement in ternary** x === y ? console.log(true) : console.log(false);

## Things I want to know more about

* I don't understand the second question of the reading. I think that maybe you would want to wait until the form is submitted to send along the result of the input form, just because it might take a more trouble than it's worth to send every keystroke through multiple functions in props. Ultimately though I'm unsure if that would even make a difference. 