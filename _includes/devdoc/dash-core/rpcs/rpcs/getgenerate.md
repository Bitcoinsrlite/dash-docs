{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_includes/devdoc/dash-core/rpcs/rpcs/getgenerate.md" %}

##### GetGenerate
{% include helpers/subhead-links.md %}

{% assign summary_getGenerate="returns if the server is set to generate coins or not." %}

{% autocrossref %}

*Requires wallet support.*

*Removed in Bitcoin Core 0.13.0.*

The `getgenerate` RPC {{summary_getGenerate}}

*Parameters: none*

*Result---whether the server is set to generate blocks*

{% itemplate ntpd1 %}
- n: "`result`"
  t: "bool"
  p: "Required<br>(exactly 1)"
  d: "Set to `true` if the server is set to generate blocks; set to `false` if it is not"

{% enditemplate %}

*Example from Dash Core 0.12.2*

{% highlight bash %}
dash-cli -regtest getgenerate
{% endhighlight %}

Result:

{% highlight json %}
false
{% endhighlight %}

*See also*

* [Generate][rpc generate]: {{summary_generate}}
* [GenerateToAddress][rpc generatetoaddress]: {{summary_generateToAddress}}
* [GetMiningInfo][rpc getmininginfo]: {{summary_getMiningInfo}}
* [SetGenerate][rpc setgenerate]: {{summary_setGenerate}}

{% endautocrossref %}
