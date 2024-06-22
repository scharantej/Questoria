## Flask Application Design for RAG Web App

### HTML Files

- **index.html**: This file will serve as the main page of the web application. It will contain an interface for the user to submit questions about websites.
- **results.html**: This file will display the results of the question asked by the user. It will show the generated answers from the vector database and the Gemini models.

### Routes

- **home**: This route will handle the user's requests for the main page (`index.html`).
- **search**: This route will process the user's question and pass it to the vector database and the Gemini models for question answering. It will then render the `results.html` page along with the generated answers.

### Flask Application Structure

```
|- app.py
|- templates
    |- index.html
    |- results.html
|- static
    |- CSS files
    |- JavaScript files
```

### Implementation Details

- The home route will use the GET method to retrieve the user's question from the `index.html` form.
- The search route will use the POST method to receive the user's question and process it.
- The search route will utilize the vector database and Gemini models to generate answers for the user's question.
- The results.html file will display the generated answers to the user.