
<blockquote>
<p>本来认为此类教程，肯定是满网飞了。今天首次使用VS Code的Git功能，翻遍了
所有中文教程，竟没有一个靠谱的。遂动笔写一篇，造福网友吧。</p>

<ul>
<li>请确保你安装了最新的VS Code.<a href="http://code.visualstudio.com/">http://code.visualstudio.com/</a></li>
<li>请确保安装了最新版的Git。<a href="https://git-scm.com/download%E3%80%82git%E5%AE%89%E8%A3%85%E5%88%B0%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F%E9%87%8C%EF%BC%8C">https://git-scm.com/download。git安装到环境变量里，</a>
确保任意路径可以访问。</li>
<li>参考链接：<a href="https://code.visualstudio.com/Docs/editor/versioncontrol">https://code.visualstudio.com/Docs/editor/versioncontrol</a></li>
</ul>
</blockquote>

<p>VS Code 集成了Git功能，并支持基本的git命令，这使得我们能够在开发过程方便的提交和获取代码。</p>

<h2><a id="user-content-11-初始化" class="anchor" href="#11-初始化" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1.1 初始化</h2>

<p>首先我们创建一个名为gittest的文件夹，当然它不在git的版本控制管理中。</p>

<p><a href="/xuanhun/vscode/blob/master/1.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/1.jpg" alt="" style="max-width:100%;"></a></p>

<p>用VS Code 打开这个文件夹，单击左侧的git图标。</p>

<p><a href="/xuanhun/vscode/blob/master/2.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/2.jpg" alt="" style="max-width:100%;"></a></p>

<p>我们可以看到“初始化GIT存储库”的按钮，单击。</p>

<p><a href="/xuanhun/vscode/blob/master/3.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/3.jpg" alt="" style="max-width:100%;"></a>
初始化之后，我们首先看到的是git栏里显示了当前所有文件，有4个更改。</p>

<p><a href="/xuanhun/vscode/blob/master/4.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/4.jpg" alt="" style="max-width:100%;"></a></p>

<p>全部或者单个文件都可以选择暂存或者清理掉。</p>

<p><a href="/xuanhun/vscode/blob/master/5.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/5.jpg" alt="" style="max-width:100%;"></a></p>

<p>在上方有提交和刷新按钮，下拉菜单里有更多选项。
再回到我们的文件中，刚才的操作创建了一个.git文件夹，放置了当前仓库的所有
配置文件，如下图。</p>

<p><a href="/xuanhun/vscode/blob/master/6.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/6.jpg" alt="" style="max-width:100%;"></a></p>

<p>到目前为止我们在本地创建了一个代码仓库，下面来看一下VS Code的git功能。</p>

<h2><a id="user-content-git-输出" class="anchor" href="#git-输出" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>git 输出</h2>

<p>我们可以在隐藏的菜单中选择git输出，这样我们每个操作都会显示
在输出区域，方便我们查看对应的git命令。</p>

<p><a href="/xuanhun/vscode/blob/master/7.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/7.jpg" alt="" style="max-width:100%;"></a></p>

<h2><a id="user-content-提交保存" class="anchor" href="#提交保存" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>提交保存</h2>

<p>提交保存的第一步是暂存文件。</p>

<p>第二步是输入提交信息。</p>

<p>第三步然后使用状态栏的提交按钮提交全部更改。</p>

<p><a href="/xuanhun/vscode/blob/master/8.png" target="_blank"><img src="/xuanhun/vscode/raw/master/8.png" alt="" style="max-width:100%;"></a></p>

<h2><a id="user-content-git命令列表" class="anchor" href="#git命令列表" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>git命令列表</h2>

<p>ctrl+shift+P，输入git，会看到VS CODE支持的所有git命令。</p>

<p><a href="/xuanhun/vscode/blob/master/9.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/9.jpg" alt="" style="max-width:100%;"></a></p>

<h3><a id="user-content-撤销操作" class="anchor" href="#撤销操作" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>撤销操作</h3>

<p>输入 Undo Last Commit，撤销上次操作。输入Unstage,撤销暂存。</p>

<p><a href="/xuanhun/vscode/blob/master/10.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/10.jpg" alt="" style="max-width:100%;"></a></p>

<h3><a id="user-content-分支" class="anchor" href="#分支" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>分支</h3>

<p>输入Branch可以创建当前内容的分支。创建分支时需要输入分支名称。</p>

<p><a href="/xuanhun/vscode/blob/master/11.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/11.jpg" alt="" style="max-width:100%;"></a>
<a href="/xuanhun/vscode/blob/master/12.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/12.jpg" alt="" style="max-width:100%;"></a></p>

<h3><a id="user-content-checkout" class="anchor" href="#checkout" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>checkout</h3>

<p>创建分支后，使用checkout命令可以拉取特定的分支内容。</p>

<p><a href="/xuanhun/vscode/blob/master/13.png" target="_blank"><img src="/xuanhun/vscode/raw/master/13.png" alt="" style="max-width:100%;"></a></p>

<h3><a id="user-content-冲突合并" class="anchor" href="#冲突合并" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>冲突合并</h3>

<p>VS Code 会检测文件冲突，并以&lt;&lt;&lt;&lt;&lt;,&gt;&gt;&gt;&gt;,====和颜色区分出来。</p>

<p><a href="/xuanhun/vscode/blob/master/14.png" target="_blank"><img src="/xuanhun/vscode/raw/master/14.png" alt="" style="max-width:100%;"></a></p>

<p>解决冲突之后，直接提交就行了。</p>

<h3><a id="user-content-文件比较" class="anchor" href="#文件比较" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>文件比较</h3>

<p>在git文件列表中，单击一个未提交更改的文件，就会打开两个窗口来显示变更的内容。</p>

<p><a href="/xuanhun/vscode/blob/master/15.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/15.jpg" alt="" style="max-width:100%;"></a></p>

<h2><a id="user-content-连接远程代码仓库" class="anchor" href="#连接远程代码仓库" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>连接远程代码仓库</h2>

<p>说了这么多，现在问题来了，在本机初始化一个代码库，一般没什么卵用。
我们大多数情况是要连接远程的代码服务器的。</p>

<p>下面我们在github上创建一个Repository，复制地址备用。</p>

<p><a href="/xuanhun/vscode/blob/master/16.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/16.jpg" alt="" style="max-width:100%;"></a>
<a href="/xuanhun/vscode/blob/master/17.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/17.jpg" alt="" style="max-width:100%;"></a></p>

<p>接下来到当前Repository文件夹根目录中，如果没有初始化过，安装文章开始初始化的方法，进行初始化。
然后执行下面的命令</p>

<div class="highlight highlight-source-shell"><pre>git remote add origin https://github.com/xuanhun/vscode.git
git pull origin master</pre></div>

<p>现在我们查看一下.git文件夹下的config文件，可以看到添加了远程Reps地址。</p>

<p><a href="/xuanhun/vscode/blob/master/18.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/18.jpg" alt="" style="max-width:100%;"></a></p>

<p>接下来我们从下拉菜单中执行发布命令。</p>

<p><a href="/xuanhun/vscode/blob/master/19.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/19.jpg" alt="" style="max-width:100%;"></a></p>

<p>这时会提醒我们输入账号和密码。</p>

<p><a href="/xuanhun/vscode/blob/master/20.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/20.jpg" alt="" style="max-width:100%;"></a></p>

<p>输入之后，会把本地提交的文件同步到github。同步之后再打开git的隐藏菜单，可以看到
同步等命令可以直接使用了。</p>

<p><a href="/xuanhun/vscode/blob/master/21.jpg" target="_blank"><img src="/xuanhun/vscode/raw/master/21.jpg" alt="" style="max-width:100%;"></a></p>

<h2><a id="user-content-简化一点的方法" class="anchor" href="#简化一点的方法" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>简化一点的方法</h2>

<p>当然我们也可以使用git 的clone命令，从远程克隆一个Reps，然后直接用vscode打开文件夹，
VS Code 会自动识别各项配置。</p>

<h3><a id="user-content-持久化账号" class="anchor" href="#持久化账号" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>持久化账号</h3>

<p>远程连接git的问题解决了，如果你不想每次同步的时候都输入账号信息，可以全局存储账号，
解决这个问题。</p>

<div class="highlight highlight-source-shell"><pre>git config --global credential.helper wincred</pre></div>

<h2><a id="user-content-小结" class="anchor" href="#小结" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>小结</h2>

<p>本文的大部分内容都能从官方的文档上找到，不过中文很多教程没有解决连接远程
服务的问题，所以特地做了说明，希望对各位有所帮助。
最后，本篇文章作为实验内容，同步到github的地址为：
<a href="https://github.com/xuanhun/vscode/blob/master/Visual%20Studio%20Code%20%E4%BD%BF%E7%94%A8Git%E8%BF%9B%E8%A1%8C%E7%89%88%E6%9C%AC%E6%8E%A7%E5%88%B6.md">VS Code 集成git</a></p>
