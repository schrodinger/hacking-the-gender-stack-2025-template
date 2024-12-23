# Hacking the Gender Stack 2025

This template can be used as a starting point for developing your own application during the hackathon. The template is a [Flask](https://flask.palletsprojects.com/en/stable/) project - you can find a quick tutorial about Flask and its best practices [here](https://flask.palletsprojects.com/en/stable/tutorial/).

## Common commands
```sh
# To install/update the project's dependencies
$> pip install -r requirements.txt

# To start the server
$> flask run
```

## Starter code

We've provided you with some starter boilerplate code that should enable your team to quickly prototype your application.

### `app.py`

The entrypoint for your flask application is in the `app.py` module. The `flask run` command is set up to automatically find and run the flask application defined in this module. You can add more modules to add additional functionality as your project needs it (like the `chemistry.py` module in the [demo](https://github.com/schrodinger/hacking-the-gender-stack-2025-demo)).

### `templates/base.html`

We've included a base Jinja template that we recommend extending in any of your own templates (learn more about extending templates [here](https://jinja.palletsprojects.com/en/stable/templates/#template-inheritance)):

```html
<!-- templates/my-template.html -->

{% extends "base.html" %}

{% block content %}
<p>
  The HTML markup for your page should be included in the 'content' block
</p>
{% endblock %}

{% block styles %}
<style>
  // Any custom CSS you may need to write should be included in a style tag within the 'styles' block
</style>
{% endblock %}

{% block scripts %}
<script>
  // Any JavaScript you write should be included in the 'scripts' block
</script>
{% endblock %}
```

The base template includes [Bootstrap](https://getbootstrap.com/), a frontend toolkit, to allow you to quickly create polished UI elements. You can learn more about Bootstrap [here](https://getbootstrap.com/docs/5.3/getting-started/introduction/). (NOTE: The base template includes a maximal bundle of Bootstrap utilities that includes all necessary modules for supporting advanced features like tooltips and [Bootstrap icons](https://icons.getbootstrap.com/))
