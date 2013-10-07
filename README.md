Jade Bootstrap - form mixins
==========================

Jade Mixins for bootstrap forms
Bootstrap v 3.0.0

Tailored for use with express-form 

Use example

Code requred to get errors and field repopulation

    var errors = req.form && req.form.getErrors() ||  {};
    var values = req.body || {};
    res.render('..register', { errors: errors, values: values });

creating the fields

    form(method='post', action='', role="form", class='form-horizontal')
		  +field-label-md('text', 'Username', 'username', 'register-display')#username-group
		  +field-label-md('email', 'Email', 'email', 'register-email')
		  +field-label-md('password', 'Password', 'password', 'register-password').banana
		  +submit('Register')

