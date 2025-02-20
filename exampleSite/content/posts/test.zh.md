---
title: "Test Page"
date: 2019-08-04T22:49:56+08:00
lastmod: 2019-08-17T22:41:56+08:00
draft: true
author: ""
authorLink: ""
description: "This is a test page."
license: ""

tags: ["Hugo", "主题"]
categories: ["预览"]
hiddenFromHomePage: false

featuredImage: ""
featuredImagePreview: ""

toc: true
autoCollapseToc: true
lightgallery: true
math: true
comment: false
---

## :(fas fa-rocket): This is a test page

[https://www.aol.com/article/entertainment/2020/02/10/oscars-viewership-hits-new-low-with-236-million-viewers/23923047/](https://www.aol.com/article/entertainment/2020/02/10/oscars-viewership-hits-new-low-with-236-million-viewers/23923047/)

Test all features in development.

<!--more-->

## Test Img

![Web Image 1](https://static.dillonzq.com/images/20190817130904-U6cPUk.jpg "Web Image")

![Local Image](/images/Apple-Devices-Preview.png "Local Image")

## Test Code

### Inline code

Inline code: `print`

### Code block with backticks

```java
class DataHolder<T>{
    T item;

    public void setData(T t) {
        this.item=t;
    }

    public T getData() {
        return this.item;
    }
}
```

```go
func (d *Database) GetCollectionByID(id uint) (*model.Collection, error) {
	var collection model.Collection
	if err := d.DB.Where("deleted = 0").
		First(&collection, id).Error; err != nil {
		return nil, err
	}
	return &collection, nil
}
```

```python
class Labels(object):
    __slots__ = ('taskid', 'labels')

    def __init__(self, taskid, labels):
        # check labels
        if isinstance(labels, str):
            labels = [labels]
        assert isinstance(labels, list), 'labels should be list'
        labels = [_check_tag(label) for label in labels]

        self.taskid = taskid
        self.labels = labels

    def for_add(self):
        return {
            'taskid': self.taskid,
            'tags': self.labels,
        }

    @property
    def token(self):
        _check_credential(self._credential)
        return self._credential['token']

def scale(scalar: float, vector: Vector) -> Vector:
    return [scalar * num for num in vector]
```

```js
_Blog.chroma = function () {
    const blocks = document.querySelectorAll('.highlight > .chroma');
    for (let i = 0; i < blocks.length; i++) {
        const block = blocks[i];
        const codes = block.querySelectorAll('pre.chroma > code');
        const code = codes[codes.length - 1];
        const lang = code ? code.className.toLowerCase() : '';
        block.className += ' ' + lang;
    }

    const nolinenosBlocks = document.querySelectorAll('.highlight > pre.chroma');
    for (let i = 0; i < nolinenosBlocks.length; i++) {
        const block = nolinenosBlocks[i];
        const chroma = document.createElement('div');
        chroma.className = block.className;
        const table = document.createElement('table');
        chroma.appendChild(table);
        const tbody = document.createElement('tbody');
        table.appendChild(tbody);
        const tr = document.createElement('tr');
        tbody.appendChild(tr);
        const td = document.createElement('td');
        tr.appendChild(td);
        block.parentElement.replaceChild(chroma, block);
        td.appendChild(block);
    }
};
```

## Test ECharts

{{< echarts >}}
title:
  text: 某站点用户访问来源
  subtext: 纯属虚构
  x: center
tooltip:
  trigger: item
  formatter: '{a} <br/>{b} : {c} ({d}%)'
legend:
  orient: vertical
  left: left
  data:
    - 直接访问
    - 邮件营销
    - 联盟广告
    - 视频广告
    - 搜索引擎
series:
  - name: 访问来源
    type: pie
    radius: 55%
    center:
      - 50%
      - 60%
    data:
      - value: 335
        name: 直接访问
      - value: 310
        name: 邮件营销
      - value: 234
        name: 联盟广告
      - value: 135
        name: 视频广告
      - value: 1548
        name: 搜索引擎
    itemStyle:
      emphasis:
        shadowBlur: 10
        shadowOffsetX: 0
        shadowColor: 'rgba(0, 0, 0, 0.5)'
{{< /echarts >}}

## Test Mermaid

{{< mermaid >}}
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
{{< /mermaid >}}

## Test Ruby

人最重要的特点是会思考，建站初衷无非是保存思维的电子快照。
当然各种文档工具亦或是简单的文本编辑器也能随时记录点滴，
选择建个人网站无非是想满足 [技术爱好者]^(Technology enthusiast) 的偏执。

## Test Music

## Test Toc

Toc

### Toc1

Toc

#### Toc 1-1

Toc

#### Toc 1-2

Toc

#### Toc 1-3

Toc

### Toc2

Toc

#### Toc 2-1

Toc

#### Toc 2-2

Toc

### Toc3

Toc

## Test Table

| Tables        | Are           | Cool  |
| :------------ |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

## Test kbd

<kbd>ctrl</kbd>+<kbd>alt</kbd>+<kbd>del</kbd>

## Test Mixed Lists

Mixed Lists

- item 1
  * [X] item A
  * [ ] item B
    more text
    1. item a
    2. itemb
    3. item c
  * [X] item C
- item 2
- item 3

Really Mixed Lists

- item 1
  * [X] item A
  - item B
    more text
    1. item a
    + itemb
    + [ ] item c
  1. item C
1. item 2
- [X] item 3

## Test fa (Font Awesome)

:(fab fa-weixin fa-2x):

## Test Footnote

This is a footnote[^1]

[^1]: https://www.aol.com/article/entertainment/2020/02/10/oscars-viewership-hits-new-low-with-236-million-viewers/23923047/

## Test Admonition

{{% admonition quote %}}
biu biu biu.
{{% /admonition %}}

{{% admonition quote "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition example "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition bug "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition danger "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition failure "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition warning "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition question "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition success "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition tip "I'm title!" false %}}
biu biu biu.
{{% /admonition %}}

{{% admonition info "I'm title!" true %}}
**biu biu biu.**
{{% /admonition %}}

{{% admonition note "I'm title!" false %}}
**biu biu biu.**
{{% /admonition %}}

{{% admonition type="abstract" title="Test Admonition" %}}
This is a Admonition.
{{% /admonition %}}

## Test Highlight

`ls` 命令

```go
// You can edit this code!
// Click here and start typing.
package main

import "fmt"

func main() {
  fmt.Println("Hello, 世界", "Hello, 世界", "Hello, 世界", "Hello, 世界", "Hello, 世界", "Hello, 世界", "Hello, 世界", "Hello, 世界")
}
```

- This is a list that contains multiple code blocks.

  - Here is an indented block

    ```Code
    This will still be parsed
    as a normal indented code block.
    ```

  - Here is a fenced code block:

    ```Code
    This will still be parsed
    as a fenced code block.
    ```

    > ```Code
    > Blockquotes?
    > Not a problem!
    > ```

## Test Typeit

{{< typeit group="test" tag="h3" >}}
Here is a story about love...
{{< /typeit >}}

{{< typeit group="test" code="java" >}}
int a = 1;
{{< /typeit >}}

## Test Align

{{% align right %}}
**Test Text**
{{% /align %}}

## Test Katex

$$ c = \pm\sqrt{a^2 + b^2} $$

Left \\( c = \pm\sqrt{a^2 + b^2} \\) Right

Left $ c = \pm\sqrt{a^2 + b^2} $ Right

$ \ce{CO2 + C -> 2 CO} $

$ \ce{Hg^2+ ->[I-] HgI2 ->[I-] [Hg^{II}I4]^2-} $
