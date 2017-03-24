# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components. Explain why each piece might be it's own component.

    ```md
I don't what this question is asking.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
  ember generate component my-map;
    ```

1.  What files are created and/or edited to produce a component, and what are their responsibilities?

    ```md
component:data template:data handlebars and test(self explanatory)
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` route. What is
    the syntax (code that is written) to render this component inside that template?

    ```html

      {{#each model as |my-contact|}}
        {{contacts my-contact=my-contact}}
        {{/each}}
    ```

1.  Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{#each model as |my-phone|}}
      {{my-contact my-phone=my-myphone}}
      {{/each}}
    ```
