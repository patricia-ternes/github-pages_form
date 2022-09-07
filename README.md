# GitHub Pages Forms 

In this repository I show a simple way of using forms in GitHub/Jekyll pages.

## Credits

- This project was inspired by [WebJeda][1].
- The form main structure and style was inspired by [W3Schools][2].
- The `html`/`email` integration is handled by [Formspree][3].

## Setting up

### Formspree Account

1. Create and validate a [Formspree][3] account.
2. Then, create a [Formspree][3] `New Form`. You will need add:
  - Form name
  - Define one email to be integrated with your form
3. After create the Formspree Form you will have access to the `form's endpoint` - keep this information.

*Note that the basic Formspree account is **Free**. You will have access up to 50 answers/month.*

#### Formspree Report

In addition to receiving an email each time the form is filled out, you can also access all data on the Formspree Report platform.

### HTML Form

Crete an `html` form that fits your needs. Then, add the Formspree endpoint link as a html form atribute.
You also need add the method="POST".

For example, if the endpoint is:

```bash
https://formspree.io/f/XXXXXXX
```

them the `html` form needs to be defined as:

```html
<form action="https://formspree.io/f/XXXXXXX" method="POST">

  <! -- form main content -->
  
</form>
```

#### Tip: Formspree Form Library

If you do not know how to create a `html` form, you can find one in the [Formspree Form Library][4].

### GitHub Pages

After having a `html` file/form you need to activate the `Github Page`. To do this:

- go to: `Settings > Pages > Build and deployment > Branch`
- select the branch where your `html` file/form is
- save, back to `<>code` tab and wait
- a github action will be automatically triggered (you may notice a small yellow circle next to the committee number). Once the circle becomes a green check mark, your form site is ready. 
- to find the website address you can go back to `Settings > Pages`- it will be listed at the top.

**It is DONE! Your form is already working.**

Go to your webpage and test your form.

## Working Example: Contact Form

As example, I created a working Contact Form available at:

- the`html` form: [index.html][5]
- the `css` layout definition (optional): [assets/css/form.css][6]
- the working GitHub [webpage][7]

[1]: https://www.youtube.com/watch?v=IP6HsgwQkvs&ab_channel=WebJeda
[2]: https://www.w3schools.com/howto/howto_css_contact_form.asp
[3]: https://formspree.io/
[4]: https://formspree.io/library/
[5]: https://github.com/patricia-ternes/github-pages_form/blob/main/index.html
[6]: https://github.com/patricia-ternes/github-pages_form/blob/main/assets/css/form.css
[7]: https://patricia-ternes.github.io/github-pages_form/

