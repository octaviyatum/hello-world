
# hello-world

Привет!

Первая проба пера.



<form id="post-new-comment" class="form" action="{{ site.staticmanUrl }}" method="post">
    <input type="hidden" name="options[slug]" value="{{ post_slug }}">
    <input type="hidden" name="options[parent]" value="{{ post_slug }}">
	<input type="hidden" name="options[origin]" value="{{ site.url }}{{ page.url }}">
	<input type="hidden" name="options[redirect]" value="{{ site.url }}{{ page.url }}">

    
    <input type="text" name="company" class="text-field" style="display: none">
	<input class="form__field text-field" type="text" name="fields[name]" placeholder="{{ site.data.language.comment_form.name }}" required/>
    <input class="form__field text-field" type="email" name="fields[email]" placeholder="{{ site.data.language.comment_form.email }}" required/>
    <input class="form__field text-field" type="url" name="fields[url]" placeholder="{{ site.data.language.comment_form.url }}"/>
    <input class="form__field text-field" type="address" name="fields[address]" placeholder="{{ site.data.language.comment_form.address }}" style="display: none"/>
    <textarea class="form__field text-field" rows="10" name="fields[message]" placeholder="{{ site.data.language.comment_form.message }}" required></textarea>
    <input class="large radius button" type="submit" value="{{ site.data.language.comment_form.send }}" /> {{ site.data.language.comment_form.send_hint }} 
</form>
