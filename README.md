# Keentivate
An _almost_ no-code Keen.js to HTML Wrapper

## Why?
Keen's javascript SDK is unfortunately complex.  Quite powerful, but unfortunately complex.  Keentivate wraps all that complexity up and turns it into a simple HTML markup syntax.  Ideally, you shouldn't have to write more than two lines of javascript!

## Install
You only need to include the `keentivate.min.js` javascript file, setup your API keys, and you're ready to rock-and-roll!

```
<script type="text/javascript" src="/js/keentivate.min.js"></script>
<script type="text/javascript">
	var keenCharts = new keentivate({
		projectId: "50f9e03d38433113c1000000", 
		readKey: "b26ea0311b271ca63c315b4ac474f5d1ed42d496b6b7fcf050d1dca3fa2ff968bbc9a3e403506322b64b07501acdaf8c22a3a70c80583a9e9a106bb7006a001b7cbf80ef5676617ffa0d530c43e435b9915a8b3f8c6809b6c97f6ff4783a383ed44ca3942b22279517fc8f959bb7e06d"
	}, 
	{
		keenClass: "keentivate"
	});
</script>
```

## HTML Syntax

You can see all of the examples on the [keentivate homepage](http://cultivatestudios.github.io/keentivate/)

In general, though, you're going to want to work with `div`s, and add a keentivate-specific class.  I usually just use `keentivate`.  You'll then apply `keen-` attributes to specify the settings for that visualization.  Below is an example of a simple pie chart.

```
 <div class="keentivate"
   data-keen-type="pie"
   data-keen-event="Plays"
   data-keen-group="play_type"
   data-keen-title="Types of Plays">
</div>
```

# Todo

I just want to make a **GIANT** note that keentivate is not thoroughly tested.  I've tested it as far as my uses go, and it works fine, but I won't in any way promise that it won't blow up in your environment.

- Test
- Documentation on differing syntax between Keen.js and keentivate
- Documentation in general

# Who?
Keentivate was built by [Joe Wegner](http://www.wegnerdesign.com) under the umbrella of [Cultivate Studios](http://www.cultivatestudios.com)

# License

Keentivate is licensed under the [MIT License](http://opensource.org/licenses/MIT)