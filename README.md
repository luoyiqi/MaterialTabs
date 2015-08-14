#MaterialTabs

A small project for Marerial Design Tabs.

This project uses  SlidingTabLayout.java & SlidingTabStrip.java from Google I/O [IOsched](https://github.com/google/iosched/tree/master/android/src/main/java/com/google/samples/apps/iosched/ui/widget) 

  ```java
 		// Creating The ViewPagerAdapter and Passing Fragment Manager, Titles fot the Tabs and Number Of Tabs.
        adapter = new ViewPagerAdapter(getSupportFragmentManager(), Titles, Numboftabs);

        // Assigning ViewPager View and setting the adapter
        pager = (ViewPager) findViewById(R.id.pager);
        pager.setAdapter(adapter);

        // Assiging the Sliding Tab Layout View
        tabs = (SlidingTabLayout) findViewById(R.id.tabs);
        tabs.setDistributeEvenly(true); // To make the Tabs Fixed set this true, This makes the tabs Space Evenly in Available width

        // Setting Custom Color for the Scroll bar indicator of the Tab View
        tabs.setCustomTabColorizer(new SlidingTabLayout.TabColorizer() {
            @Override
            public int getIndicatorColor(int position) {
                return getResources().getColor(R.color.tabsScrollColor);
            }
        });

        // Setting the ViewPager For the SlidingTabsLayout
        tabs.setViewPager(pager);
```

[![MaterialTabs](https://github.com/scionoftech/MaterialTabs/blob/Development/tabs.PNG)]
## License

  [ISC](LICENSE)