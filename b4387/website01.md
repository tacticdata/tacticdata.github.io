#### Build a website like this

To build a similar webste https://www.hilltopsight.com, with a navigation bar, an image called "hero image" and a content page, almost free on github.com.

The intention here is set this website as mostly a land page, when you do online advertising like Google Ads or Facebook Ads to point to the landing page, then you mention the details on the landing page, and monitoring the visiting data to your landing page,by connect your website with Google Analytics, to comparing with your history data, you sales performences, you will get a conclution whether your sales volumns,your new costumers acquisitions and media selection as wuch as you expected.That finish an online sale loop.

#### Login to github.com

You have to have a [github.com](https://github.com/) account, or go to [sign up](https://github.com/) one for free.

#### Template of website

Copy "bulma clean rheme" by click 'Fork'(on top right of the screen) https://github.com/chrisrhymes/bulma-clean-theme

#### Configure website

1. change neme of your website repository by 'Settings' --> 'Repository name' to yourusername.github.io -->  click 'Rename' button
2. set up _config.yml, by clicking the file under root location, 
	baseurl: ""
    url: "https://yourusername.github.io"
	google_analytics: UA-xxxxxxxxxxx
3. You can visit website by https://yourusername.github.io

#### navigation bar

- Location: root --> _data --> navigation.yml

You can edit as much as you need,be careful the format

The color of the navigation bar settings locate at assets/css/app.scss, mentioned in bulma-clean-theme [documentation](https://github.com/chrisrhymes/bulma-clean-theme#sidebar-visibility)

- title: Appear on top left of navigation bar and as website title, locate as `title` in _config.yml
- `Home` location: root --> _includs --> header.html line number 16

#### image hero

mentioned in called `formator` like this:

    ---
    title: 
    subtitle: some-headline
    hero_height: is-medium
    hero_image: /img/imgpath.jpg
    layout: page
    published: true
    ---

It will appear on the beginning section of a page,  we will introduct along with content page.

#### content page

- the image hero or image next to navigation bar will be defined on `formator` , example formator shown in last paragraph.
- next to the `formator`, there appears content, write as you will
- the path equal to url,the content page should be in .md eg. markdown format,  if you want to put page on root level,you can put on root,along side with index.md, if you want to put on second level, put the page in a folder, for example, https://yourusername.github.io/example-folder/example-page.htm access `example-page` in `example-folder` folder, that is defined by _config.yml on permalink: pretty with format as /example-folder/example-page/

#### migrating website to Netlify.com (optional)

In case you want to host the github.com repository to Netlify.com, there are few steps:

- step 1: login with github account by Login https://app.netlify.com/  click `Github` --> `New site from Git` --> `Github` --> `Select from specific repository` --> yourusername/yourusername.github.io --> `Build options, and deploy!`
- step 2: Before you click `Depoy site` button, 
		- add following line `gem 'github-pages'` below `source "https://rubygems.org"` on `Gemfile`
        - create a `.ruby-version` on rooot then fill `2.4.3`in it
        - refer to: https://www.netlify.com/blog/2017/05/11/migrating-your-jekyll-site-to-netlify/
- step 3: click `Depoy site` button, disable block ads extension if availible.

#### custom domain name

- step 1: You have to buy a domain name, surpose it is called 'example.com', you want to visit via 'www.example.com', for instance, the domain name we use cost about USD 6.00 first year, may slighly higher next year.
- step 2: login your github.com account
- step 3: go to `Settings` --> `Custom domain` put www.example.com in the box then `Save`, the github automatically create a file under root called 'CNAME'
- step 4: go to set up DNS CNAME redirection,surpose to be like www.example.com redirect to yourusername.github.io
- step 5: check `Settings` --> `Enforce HTTPS` 
- step 6: access website with https://www.example.com


#### The structure of a website

- Methodology

	- modular
    - layers
    - data in mind
    
Inmagine every elements in website can be assembled.

- Structure
	- navigation bar
    - image hero
    - content page
    
A content page is the fundamental element, depend on the content it purposes for.

#### The object of  website

- The website will not automatically bring traffic
- The best way to promote is through online advertising
- It apply the nature of competition in business
