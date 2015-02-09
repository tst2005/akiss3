# What is AKISS 3.1

It's pseudo-random generator, found on the [Result Page](http://www.cacert.at/cgi-bin/rngresults) of a [Random Number Generator Analysis WebSite](http://www.cacert.at/random/).

The AKISS3.1 seems good.


# Original Source Code

I found his source code on http://besides.us/posts/5
But this website seems to be destroyed by spammers/virus...

The original post :

```
AKISS 3.1

By admin|C#, programming|Be the first to comment!

public sealed class AKISS
{
	ulong _a = 0x6cd2d2bab6fb1b, _b = 0x42fc73c2ace698ad, _c = 0x2b20cc237775d265;
	public ulong NextUlong()
	{
		_a = _b + ((_a << 7) | (_c >> 57));
		_b = _c ^ ((_c << 13) | (_a >> 51));
		return _c = _a - ((_b << 17) | (_b >> 44));
	}
}
```

