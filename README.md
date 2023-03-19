# Console-Log-Port
A svelte component which helps you log on the console using a styled input field because why not :cat:. To use it import the component and add this line:
`<ConsolePort on:enter={(e) => console.log(e.detail.textToDisplay)}/>`.
This tag will allow the input from the input field to log onto the console
