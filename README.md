Android ViewPagerIndicatorView
===========================

An android tab indicator with viewpager easy to use!

Step:

1.in android layout:
{% highlight xml %}
<com.app.library.common.view.ViewPagerIndicatorView
        android:id="@+id/viewpager_indicator_view"
        android:layout_width="match_parent"
        android:layout_height="wrap_content" />
{% endhighlight %}


2.in java code:
{% highlight java %}
ViewPagerIndicatorView viewPagerIndicatorView; = (ViewPagerIndicatorView) findViewById(R.id.viewpager_indicator_view);

final Map<String, View> map = new HashMap<String, View>();
map.put("TAB1", LayoutInflater.from(this).inflate(R.layout.activity_sample_pager_0, null));
map.put("TAB2", LayoutInflater.from(this).inflate(R.layout.activity_sample_pager_1, null));

viewPagerIndicatorView.setupLayout(map);
{% endhighlight %}
