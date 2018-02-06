# Document Format

在每一個Project當中，無可避免的我們都有很多的文件要寫。

目前常見到的文件格式，有 Word, Latex, Markdown, HTML, PowerPoint。在這些格式當中，我們到底應該使用哪一種格式與工具呢?

### 各種格式的特色

在回答這個問題之前，我們先來看一下各種格式的特色：

##### Office 系列

最多人使用，尤其是 MS Office，其他像是 Mac 跟 LibreOffice 都有一定的使用者。

優點是強大的圖形介面與各種強大的排版功能，甚至有許多圖片處理的功能在裡面。

缺點是產生的檔案都是類似 Binary 的檔案，難以對這類型格式進行版本控制，而且無法同時後對多個文件檔案進行字串搜尋，這以後會對大量文件管理造成困擾。另外就是要看這些文件，該電腦一定要有相對應的軟體，如 MS-Office，還要注意版本相容性。

所有的 Office 系列都具有以上的問題，唯一一個例外就是 Google Doc，幾乎克服了上述的所有缺點，但是 Google Doc 的缺點在於他是雲端服務，無法在自己的電腦上擁有一份。

##### Latex

寫論文專用，歷史悠久的文件格式，資工系同學尤其愛用，特色為寫文件寫起來像是在寫程式一樣。

缺點是可讀性較差，對於非資工系的同學來說，有點不夠親切。

但是優點是印出來的文件非常漂亮，並且發展多年，擁有許多強大的 Plugin，像是僅需要將資料點的座標標出來，就可以畫出精美的 Dotplot 或是其他類型的圖表。

此外，原始檔是使用 plain text 的形式，因此文件內所有的內容，包含排版資訊，像是頁面的上下間距，都可以進行版本控制跟多檔搜尋。

##### Markdown

介於 Latex 與 Office 中間，檔案格式為plain text，易於做版本控制跟多檔搜尋。優點是容易上手，缺點則是功能較少。不論是Office 或是 Latex，擁有的功能都遠超過 markdown。

Markdown 的文件內容很單純，檔案很小，所有的內容都是文章內容，不會有頁面間距、行距、字型等等的頁面排版訊息。

他所擁有的就是大標題、小標題與各級標題，或者是清單、表格之類，都是跟你的文章的實際內容有關的功能。

Markdown 算是一種文件格式，所以說網路上支援各式各樣的編輯器來編輯 Markdown ，有些編輯器還支援一些 extension，在 Markdown 之外再多加一些功能，讓你能夠除了基本功外能還能多做一些像是繪製圖表之類的事。

### 如何使用 Markdown 

根據維基百科的介紹：

> [John Gruber](https://en.wikipedia.org/wiki/John_Gruber) created the Markdown language in 2004 in collaboration with [Aaron Swartz](https://en.wikipedia.org/wiki/Aaron_Swartz) on the syntax,[[3\]](https://en.wikipedia.org/wiki/Markdown#cite_note-markdown-swartz-3)[[4\]](https://en.wikipedia.org/wiki/Markdown#cite_note-gruber-2004-release-4) with the goal of enabling people "to write using an easy-to-read, easy-to-write plain text format, and optionally convert it to structurally valid [XHTML](https://en.wikipedia.org/wiki/XHTML) (or [HTML](https://en.wikipedia.org/wiki/HTML))".[[5\]](https://en.wikipedia.org/wiki/Markdown#cite_note-md-5)
>
> The key design goal is *readability* – that the language be readable as-is, without looking like it has been marked up with tags or formatting instructions,[[9\]](https://en.wikipedia.org/wiki/Markdown#cite_note-philosophy-9) unlike text formatted with a [markup language](https://en.wikipedia.org/wiki/Markup_language), such as [Rich Text Format](https://en.wikipedia.org/wiki/Rich_Text_Format) (RTF) or HTML, which have obvious tags and formatting instructions. To this end, its main inspiration is the existing [conventions](https://en.wikipedia.org/wiki/Convention_(norm)) for marking up [plain text](https://en.wikipedia.org/wiki/Plain_text) in [email](https://en.wikipedia.org/wiki/Email), though it also draws from earlier markup languages, notably [setext](https://en.wikipedia.org/wiki/Setext), [Textile](https://en.wikipedia.org/wiki/Textile_(markup_language)), and [reStructuredText](https://en.wikipedia.org/wiki/ReStructuredText).

Markdown 是一種易讀易寫的格式。並且許多網站都支援將 Markdown 直接排版顯示在網頁上，像是 [Github](https://guides.github.com/features/mastering-markdown/)。

Markdown 支援的編輯器很多，有的則是在編輯器上面加入 Plugin 以支援許多 Markdown 的功能。

以下介紹一些用來製作 Markdown 文件跟投影片的軟體：

**Typora**，一個相當漂亮、簡單好用的 Markdown 編輯器，跨平台支援 Linux, Mac 與 Windows。這其實是一個要收費的商業軟體，只是現在 beta 版是免費的。

**vs-code**，一個現在很受歡迎的 open source 程式碼編輯器，整合了許多的 extension，其中也有許多跟 Markdown 相關的 extension 可以使用。

**Marp** ，一個跨平台的 open source 軟體，能夠利用 Markdown 的語法來製作 PDF 投影片。

**remark** ，是一個 Javascript 程式庫，他能夠將 Markdown 轉成 html slide。

**Hugo**，一個靜態網站產生器，他提供許多好看的 Theme 供你選擇，並讓你用 Markdown 來撰寫網站內容。

**Pandoc**，能夠在許多不同格式的文件進行轉換。

### QA

- Q: Markdown 既然可以用來製作文件跟投影片，那麼能不能夠一份檔案同時用來當作文件跟投影片呢？

  A: 以目前的發展狀況來說，還是將文件跟投影片分為兩個不同的檔案比較好。因為投影片需要利用"---"來分頁，但是在文件上這些"---"是不必要的符號，並且投影片可能不會完整採用原本文件的內容。

  ​