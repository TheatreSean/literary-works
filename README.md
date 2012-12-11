# Literary Works
====================

Schema.org lacks microdata specific towards literary works - that are not in book form - published on websites. The purpose of this public endeavor is to codify and uniformly introduce microdata that will benefit all authors.

[Schema.org](http://schema.org) offers a simple method for extending their core microdata classes and properties. [The Type Hierarchy](http://schema.org/docs/full.html) shows the current microdata hierarchy in a single file.

Literary Works are extensions to the core CreativeWork class. These extensions are used with HTML5 or RDFa attributes in conjunction with existing CreativeWork properties.

These extensions are allowed and encouraged by the Schema.org  [Extension Mechanism](http://schema.org/docs/extension.html) :

>"Therefore, schema.org has created an extension mechanism that lets webmasters and developers extend our existing schemas. When you extend our schemas and use these extensions to mark up your data, search applications can at least partially understand your markup and use the data appropriately.

>"(Of course, you can always create new schemas that are not at all tied to those on schema.org, and you should do this if the content of your domain is not covered by any of the schema.org types. If the schema gains adoption and proves useful to search applications, search engines may start using this data.)

>"Extensions that gain significant adoption on the web may be moved into the core schema.org vocabulary, so that search engines can provide more functionality based on better understanding of the structured data."


## Extensions
====================
The following are the currently proposed extensions. However, it is by no means complete.


### Literary (Main Class)
====================
* ```http://schema.org/CreativeWork/LiteraryWork```

### Story
====================
* ```http://schema.org/CreativeWork/LiteraryWork/Story```
* ```http://schema.org/CreativeWork/LiteraryWork/Story/storyChapter```
* ```http://schema.org/CreativeWork/LiteraryWork/ShortStory```
* ```http://schema.org/CreativeWork/LiteraryWork/Parable```
* ```http://schema.org/CreativeWork/LiteraryWork/Fable```
* ```http://schema.org/CreativeWork/LiteraryWork/FolkTale```
* ```http://schema.org/CreativeWork/LiteraryWork/Prose```

### Poetry
====================
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Poem```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Ideogramme```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Rhyme```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Verse```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/BlankVerse```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/FreeVerse```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/ConcreteVerse```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Sonnet```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Couplet```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Ballad```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Haiku```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Tanka```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Limerick```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Ode```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Ghazal```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Villanelle```
* ```http://schema.org/CreativeWork/LiteraryWork/Poetry/Shi```

### Nonfiction
====================
* ```http://schema.org/CreativeWork/LiteraryWork/Epistle```
* ```http://schema.org/CreativeWork/LiteraryWork/Memoir```
* ```http://schema.org/CreativeWork/LiteraryWork/Biography```
* ```http://schema.org/CreativeWork/LiteraryWork/Autobiography```
* ```http://schema.org/CreativeWork/LiteraryWork/Essay```
* ```http://schema.org/CreativeWork/LiteraryWork/Elegy```
* ```http://schema.org/CreativeWork/LiteraryWork/Satire```

### Theatrical
====================
* ```http://schema.org/CreativeWork/LiteraryWork/Play```
* ```http://schema.org/CreativeWork/LiteraryWork/Play/playAct```
* ```http://schema.org/CreativeWork/LiteraryWork/Play/playScene```
* ```http://schema.org/CreativeWork/LiteraryWork/Play/musicalBook```
* ```http://schema.org/CreativeWork/LiteraryWork/SongLyric```
* ```http://schema.org/CreativeWork/LiteraryWork/Libretto```


## Examples - Microdata + HTML 5
====================
### Used in a sentence:
```
<p itemscope itemtype="http://schema.org/CreativeWork/LiteraryWork/FreeVerse">
  <span itemprop="name" lang="fr">Un Coup de Dés Jamais N'Abolira Le Hasard</span>—
  <link itemprop="url" href="http://coupdedes.com/">
  by <span itemprop="author" lang="fr">Stéphane Mallarmé</span> is one of the finest examples of free verse.
</p>
```

### Used in a navigation link:
```
[ ... ]
<li>
<b><span lang=fr>VERS</span></b> : <span itemscope itemtype="http://schema.org/CreativeWork/LiteraryWork/Story/Chapter"><a href="/oculus/1/1#oculusWorkTitle-page" itemprop="name">Zo&#235;; or, On the Clockwork Spheres of Paradise [<span lang=fr>Notre-Dame-de-Gr&#226;ce</span>]</a></span>.
</li>
[ ... ]
```

### Used in a single page:
```
<div itemscope itemtype="http://schema.org/CreativeWork/LiteraryWork">
<p><span itemprop="name">Ozymandias</span><br>
by <span itemprop="author">Percy Bysshe Shelley</span><br>
[Published <meta itemprop="datePublished" content="1818-01-11">January 11, 1818]</p>
<p itemscope itemtype="http://schema.org/CreativeWork/LiteraryWork/Poetry/Sonnet"> 
I met a traveller from an antique land<br>
Who said: Two vast and trunkless legs of stone<br>
Stand in the desert...Near them, on the sand,<br>
Half sunk, a shattered visage lies, whose frown,<br>
And wrinkled lip, and sneer of cold command,<br>
Tell that its sculptor well those passions read<br>
Which yet survive, stamped on these lifeless things,<br>
The hand that mocked them, and the heart that fed:<br>
And on the pedestal these words appear:<br>
"My name is Ozymandias, king of kings:<br>
Look on my works, ye Mighty, and despair!"<br>
Nothing beside remains. Round the decay<br>
Of that colossal wreck, boundless and bare<br>
The lone and level sands stretch far away.<p>
</div>
```


## License
==============

This work is licensed under a [Creative Commons Attribution 3.0 Unported License](http://creativecommons.org/licenses/by/3.0/deed.en_US) .