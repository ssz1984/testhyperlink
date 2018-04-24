~~~~~~~~~~~~~~~~~~~~~~~~~~
超链接（hyperlink）
~~~~~~~~~~~~~~~~~~~~~~~~~~

外部链接（external hyperlink）
==================================
方式一::

  我们推荐您点击，参考网站_.

   .. _参考网站:http://www.python.org/

页面效果：
 我们推荐您点击，参考网站_.
  .. _参考网站: http://www.python.org/

方式二：在链接名后直接列出网址，如下
 我们推荐您点击，*参考网站* <http://www.python.org/>。

内部链接（internal hyperlink）
================================
示例::

 Internal crossreferences, like example_.

 .. _example: This is an example crossreference target.

页面效果：
 Internal crossreferences, like example_.

 .. _example:

 This is an example crossreference target.

间接超链接（indirect hyperlink）
=================================
间接超链接在其链接块中具有链接指向的作用。 在以下示例中，目标“one”间接引用目标“two”所引用的内容；目标“two”引用目标为“three”，一个内部超链接目标。 实际上三者引用的是同一内容。示例::

.. _one: two_
.. _two: three_
.. _three:

说明：
如果在链接块中使用了短语引用（phrase-reference），则必须用反引号将它括起来。 与外部超链接一样，间接超链接可以从下一行或显式标记的同一行开始。 它也可以分成多行，此时前面要加空白之后该行才能被标准化。

隐式链接（implicit hyperlink）
==============================================================================================
隐式链接是指章节标题、脚注和引文自动生成的超链接，即标题文本或脚注/引用标签用作超链接名称。
----------------------------------------------------------------------------------------------

示例::

 Titles are targets, too 
 -------------------------
 Implict references, like `Titles are targets, too`_.

页面效果：

Titles are targets, too 
-------------------------
Implict references, like `Titles are targets, too`_.