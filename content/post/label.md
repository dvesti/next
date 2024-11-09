---
title: Label
description: NexT User Docs – NexT Supported Tags – Label
date: '2024-03-01'
---

### Usage

```jinja
{% label [class]@text %}
```

- `[class]` : *Optional parameter.* Supported values: `default` | `primary` | `success` | `info` | `warning` | `danger`.
  If not specified, the default style of the browser will be used, which may be different in different browsers.
- `text`    : `@text` can be specified with or without space
  E.g. `success @text` is the same as `success@text`.

### Examples

```jinja
Lorem {% label @ipsum %} {% label primary@dolor sit %} amet, consectetur {% label success@adipiscing elit, %} sed {% label info@do eiusmod %} tempor incididunt ut labore et dolore magna aliqua.

Ut enim *{% label warning @ad %}* minim veniam, quis **{% label danger@nostrud %}** exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate ~~{% label default @velit %}~~ <mark>esse</mark> cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

Lorem {% label @ipsum %} {% label primary@dolor sit %} amet, consectetur {% label success@adipiscing elit, %} sed {% label info@do eiusmod %} tempor incididunt ut labore et dolore magna aliqua.

Ut enim *{{</* label warning @ad */>}}* minim veniam, quis **{% label danger@nostrud %}** exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate ~~{% label default @velit %}~~ <mark>esse</mark> cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<div class="alert alert-primary" role="alert">
  A simple primary alert—check it out!
</div>
<div class="alert alert-secondary" role="alert">
  A simple secondary alert—check it out!
</div>
<div class="alert alert-success" role="alert">
  A simple success alert—check it out!
</div>
<div class="alert alert-danger" role="alert">
  A simple danger alert—check it out!
</div>
<div class="alert alert-warning" role="alert">
  A simple warning alert—check it out!
</div>
<div class="alert alert-info" role="alert">
  A simple info alert—check it out!
</div>
<div class="alert alert-light" role="alert">
  A simple light alert—check it out!
</div>
<div class="alert alert-dark" role="alert">
  A simple dark alert—check it out!
</div>

<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>


This is a regular paragraph.

## Note ##

{{< note title="Note" color="primary" >}}
This is an out of context note that you want to draw a users attention to.
{{< /note >}}

```markdown
{{</* note warning */>}}
  ### Warning Header
  **Welcome** to [Hugo NexT!](https://preview.hugo-next.eu.org)
{{</* /note */>}}
```


{{< note warning >}}
  ### Warning Header
  **Welcome** to [Hugo NexT!](https://preview.hugo-next.eu.org)
{{< /note >}}

## Button ##

<button type="button" class="btn btn-primary position-relative">
  Inbox
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    99+
    <span class="visually-hidden">unread messages</span>
  </span>
</button>

## Badge ##

### 1 ###

<span class="badge text-bg-primary">Primary</span>
<span class="badge text-bg-secondary">Secondary</span>
<span class="badge text-bg-success">Success</span>
<span class="badge text-bg-danger">Danger</span>
<span class="badge text-bg-warning">Warning</span>
<span class="badge text-bg-info">Info</span>
<span class="badge text-bg-light">Light</span>
<span class="badge text-bg-dark">Dark</span>

### 2 ###

<span class="badge rounded-pill text-bg-primary">Primary</span>
<span class="badge rounded-pill text-bg-secondary">Secondary</span>
<span class="badge rounded-pill text-bg-success">Success</span>
<span class="badge rounded-pill text-bg-danger">Danger</span>
<span class="badge rounded-pill text-bg-warning">Warning</span>
<span class="badge rounded-pill text-bg-info">Info</span>
<span class="badge rounded-pill text-bg-light">Light</span>
<span class="badge rounded-pill text-bg-dark">Dark</span>


### BTN ###

<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>

## Цитата ##

```shell
{{/*< quote >*/}}
  ### block quote
  写下你想表达的话语！
{{/*< /quote >*/}}
```

{{< quote >}} 
### block quote ### 
Цитата из Великих...  Ну и цитату сделали: никуда не годится! Хотя...  
Выше был код -- исправил  
    --- А почему по центру?
{{< /quote >}}

## Из Freemind ##

<h3 id="Results"><a href="#Results" class="headerlink" title="Results"></a>Results</h3><p class="text-muted">Fusce dapibus, tellus ac cursus commodo, tortor mauris nibh.</p>

<p class="text-primary">Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
<p class="text-success">Duis mollis, est non commodo luctus, nisi erat porttitor ligula.</p>

<p class="text-info">Maecenas sed diam eget risus varius blandit sit amet non magna.</p>
<p class="text-warning">Etiam porta sem malesuada magna mollis euismod.</p>

<p class="text-danger">Donec ullamcorper nulla non metus auctor fringilla.</p>
<h2 id="Buttons"><a href="#Buttons" class="headerlink" title="Buttons"></a>Buttons</h2><p>Inserts a button with target links, text and specified color.</p>
<h3 id="Syntax-1"><a href="#Syntax-1" class="headerlink" title="Syntax"></a>Syntax</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div></pre></td><td class="code"><pre><div class="line">&#123;% btn url text [style] %&#125;</div></pre></td></tr></table></figure>
<h3 id="Examples-1"><a href="#Examples-1" class="headerlink" title="Examples"></a>Examples</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div><div class="line">2</div><div class="line">3</div><div class="line">4</div><div class="line">5</div><div class="line">6</div><div class="line">7</div><div class="line">8</div><div class="line">9</div><div class="line">10</div><div class="line">11</div></pre></td><td class="code"><pre><div class="line">&#123;% btn http://hahack.com hahack %&#125;</div><div class="line"></div><div class="line">&#123;% btn http://hahack.com hahack primary %&#125;</div><div class="line"></div><div class="line">&#123;% btn http://hahack.com hahack success %&#125;</div><div class="line"></div><div class="line">&#123;% btn http://hahack.com hahack warning %&#125;</div><div class="line"></div><div class="line">&#123;% btn http://hahack.com hahack danger %&#125;</div><div class="line"></div><div class="line">&#123;% btn http://hahack.com hahack info %&#125;</div></pre></td></tr></table></figure>
<h3 id="Results-1"><a href="#Results-1" class="headerlink" title="Results"></a>Results</h3><a class="btn btn-default" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<a class="btn btn-primary" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<a class="btn btn-success" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<a class="btn btn-warning" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<a class="btn btn-danger" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<a class="btn btn-info" href="http://hahack.com" target="_blank" rel="external">hahack</a>
<h2 id="Labels"><a href="#Labels" class="headerlink" title="Labels"></a>Labels</h2><p>Inserts a label with text and specified color.</p>
<h3 id="Syntax-2"><a href="#Syntax-2" class="headerlink" title="Syntax"></a>Syntax</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div></pre></td><td class="code"><pre><div class="line">&#123;% label text [style] %&#125;</div></pre></td></tr></table></figure>
<h3 id="Examples-2"><a href="#Examples-2" class="headerlink" title="Examples"></a>Examples</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div><div class="line">2</div><div class="line">3</div><div class="line">4</div><div class="line">5</div><div class="line">6</div><div class="line">7</div><div class="line">8</div><div class="line">9</div><div class="line">10</div><div class="line">11</div></pre></td><td class="code"><pre><div class="line">&#123;% label default %&#125;</div><div class="line"></div><div class="line">&#123;% label warinng warning %&#125;</div><div class="line"></div><div class="line">&#123;% label success success %&#125;</div><div class="line"></div><div class="line">&#123;% label danger danger %&#125;</div><div class="line"></div><div class="line">&#123;% label primary primary %&#125;</div><div class="line"></div><div class="line">&#123;% label info info %&#125;</div></pre></td></tr></table></figure>
<h3 id="Results-2"><a href="#Results-2" class="headerlink" title="Results"></a>Results</h3><span class="label label-default">default</span>
<span class="label label-warning">warinng</span>
<span class="label label-success">success</span>
<span class="label label-danger">danger</span>
<span class="label label-primary">primary</span>
<span class="label label-info">info</span>
<h2 id="Badges"><a href="#Badges" class="headerlink" title="Badges"></a>Badges</h2><p>Inserts a badge with text.</p>
<h3 id="Syntax-3"><a href="#Syntax-3" class="headerlink" title="Syntax"></a>Syntax</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div></pre></td><td class="code"><pre><div class="line">&#123;% badge text %&#125;</div></pre></td></tr></table></figure>
<h3 id="Examples-3"><a href="#Examples-3" class="headerlink" title="Examples"></a>Examples</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div></pre></td><td class="code"><pre><div class="line">&#123;% badge 42 %&#125;</div></pre></td></tr></table></figure>
<h3 id="Results-3"><a href="#Results-3" class="headerlink" title="Results"></a>Results</h3><span class="badge">42</span>
<h2 id="Alerts"><a href="#Alerts" class="headerlink" title="Alerts"></a>Alerts</h2><p>Inserts alert messages with text and specified color.</p>
<h3 id="Syntax-4"><a href="#Syntax-4" class="headerlink" title="Syntax"></a>Syntax</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div><div class="line">2</div><div class="line">3</div></pre></td><td class="code"><pre><div class="line">&#123;% alert [style] %&#125;</div><div class="line">   Alert string</div><div class="line">&#123;% endalert %&#125;</div></pre></td></tr></table></figure>
<h3 id="Examples-4"><a href="#Examples-4" class="headerlink" title="Examples"></a>Examples</h3><figure class="highlight plain"><table><tr><td class="gutter"><pre><div class="line">1</div><div class="line">2</div><div class="line">3</div><div class="line">4</div><div class="line">5</div><div class="line">6</div><div class="line">7</div><div class="line">8</div><div class="line">9</div><div class="line">10</div><div class="line">11</div><div class="line">12</div><div class="line">13</div><div class="line">14</div><div class="line">15</div></pre></td><td class="code"><pre><div class="line">&#123;% alert warning %&#125;</div><div class="line">Best check yo self, you&apos;re not looking too good.</div><div class="line">&#123;% endalert %&#125;</div><div class="line"></div><div class="line">&#123;% alert danger %&#125;</div><div class="line">Change a few things up and try submitting again.</div><div class="line">&#123;% endalert %&#125;</div><div class="line"></div><div class="line">&#123;% alert success %&#125;</div><div class="line">You successfully read this important alert message.</div><div class="line">&#123;% endalert %&#125;</div><div class="line"></div><div class="line">&#123;% alert info %&#125;</div><div class="line">This alert needs your attention, but it&apos;s not super important.</div><div class="line">&#123;% endalert %&#125;</div></pre></td></tr></table></figure>
<h3 id="Results-4"><a href="#Results-4" class="headerlink" title="Results"></a>Results</h3><div class="alert alert-warning"><i class="fa fa-bell"></i>  Best check yo self, you're not looking too good.</div>
<div class="alert alert-danger"><i class="fa fa-bug"></i>  Change a few things up and try submitting again.</div>
<div class="alert alert-success"><i class="fa fa-lightbulb-o"></i>  You successfully read this important alert message.</div>
<div class="alert alert-info"><i class="fa fa-info"></i>  This alert needs your attention, but it's not super important.</div>

### Outline Buttoms ###	  
	  
<button type="button" class="btn btn-outline-primary">Primary</button>
<button type="button" class="btn btn-outline-secondary">Secondary</button>
<button type="button" class="btn btn-outline-success">Success</button>
<button type="button" class="btn btn-outline-danger">Danger</button>
<button type="button" class="btn btn-outline-warning">Warning</button>
<button type="button" class="btn btn-outline-info">Info</button>
<button type="button" class="btn btn-outline-light">Light</button>
<button type="button" class="btn btn-outline-dark">Dark</button>	  


<div class="btn-group" role="group" aria-label="Basic mixed styles example">
  <button type="button" class="btn btn-danger">Left</button>
  <button type="button" class="btn btn-warning">Middle</button>
  <button type="button" class="btn btn-success">Right</button>
</div>

<p><a href="#" class="link-primary">Primary link</a></p>
<p><a href="#" class="link-secondary">Secondary link</a></p>
<p><a href="#" class="link-success">Success link</a></p>
<p><a href="#" class="link-danger">Danger link</a></p>
<p><a href="#" class="link-warning">Warning link</a></p>
<p><a href="#" class="link-info">Info link</a></p>
<p><a href="#" class="link-light">Light link</a></p>
<p><a href="#" class="link-dark">Dark link</a></p>
<p><a href="#" class="link-body-emphasis">Emphasis link</a></p


<button type="button" class="note button-primary">Primary</button>
<button type="button" class="button note-secondary">Secondary</button>
<button type="button" class="button btn-success">Success</button>
<button type="button" class="btn button-danger">Danger</button>
<button type="button" class="button btn-warning">Warning</button>
<button type="button" class="button button-info">Info</button>
<button type="button" class="button btn-light">Light</button>
<button type="button" class="btn button-dark">Dark</button>

<button type="button" class="button btn-link">Link</button>


