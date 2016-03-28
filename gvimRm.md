![space pic](/public/images/space.jpg "space pic")

# gVim 操作命令

    查找命令
> 命令模式下，按‘/’，然后输入要查找的字符，Enter。即：/ words <br />
> ? 向前（下）查找。<br />
> / 向后（上）查找。
> n 表示按着当前的搜索方向往下查找。
> N 表示按着当前的搜索方向往上查找。


    常用命令
> % 跳转到配对的括号去<br />
> [[ 跳转到代码块的开头去(但要求代码块中'{'必须单独占一行)<br />
> gD 跳转到局部变量的定义处<br />
> '' 跳转到光标上次停靠的地方, 是两个', 而不是一个"<br />
> mx 设置书签,x只能是a-z的26个字母<br />
> `x 跳转到书签处("`"是1左边的键)<br />
> \> 增加缩进,"x>"表示增加以下x行的缩进<br />
> < 减少缩进,"x<"表示减少以下x行的缩进
>
> h 在当前行向左移动一个字符，或者Backspace。
> j 移动到下一行，或者Enter。
> k 移动到上一行，或者- 号。
> l 在当前行向右移动一个字符，或者空格键Space。
>
> yy|2yy 复制行
> dd|2dd 删除、剪切行
> p      粘贴到下一行
> P      粘贴到上一行
> ^|$    定位到行首|行尾
> dG     从当前行删到文档最后一行
>
> Ctrl +f 向前滚动一页，或者PageDown。
> Ctrl +b 向后滚动一页，或者PageUp。
> 0(零) 移至行首（包含空白字符，如缩进的空格），或是Home 键。
> $ 移至行尾， 或End 键。
> ^ 移到行首第一个非空白字符。
> G 移动到文档末尾，或者
> gg 移动到文档开头。
>
> w 移动到下一word的开头。
> b 移动到上一word的开头。
> e 移动到本word或者下个word的末尾。
> ge 移动到上个word的末尾。
> 大写的W B E 和w b e 效果一样但会忽略像. - 等特殊字符。
>
> 中文因为是连在一起的，所以如果没有空格或者数字、英文标点的话，将视为一个word。
> ( 光标移至句首，句子是以. ? ! 标点来判断的。
> ) 光标移至句尾
> { 光标移至段落的开头，段落是以空白行来判断的。
> } 光标移至段落的结尾
> H 将光标移至屏幕顶第一个非空白字符。
> M 光标移至屏幕中间第一个非空白字符。
> L 光标移至屏幕底第一个非空白字符。这和PageDown，PageUp 不一样，内文内容并未动，只是光标在动而已。
> :n 将光标定位到第n行。
> n| 将光标移动到本行第n个字符。



    Ctags 插件安装
> 下载地址：http://ctags.sourceforge.net/ <br />
> 下载地址：http://downloads.sourceforge.net/project/ctags/ctags/5.8/ctags58.zip <br />
> 在解压后将文件夹中的ctags.exe复制到D:\ProgramFiles\Vim\vim73下，并编辑_vimrc文件，添加以下内容： <br />
> set tags=tags; <br />
> set autochdir <br />
> 然后将D:\ProgramFiles\Vim\vim73加到环境变量的path中。
> 再打开 cmd ，输入 ctags -R,会生成一个 tags 文件

    taglist 插件安装
> 下载地址：https://github.com/vim-scripts/taglist.vim
> 解压后得到 doc 和 plugin 两个文件夹，将里面的内容复制到 vim 的对应文件夹中
> 在vimrc中添加设置taglist的设置：<br />
> let Tlist_WinWidth=25<br />
> let Tlist_Show_One_File=1<br />
> let Tlist_Exit_OnlyWindow=1<br />
> let Tlist_Use_Right_Window=1<br />
> let Tlist_File_Fold_Auto_Close=1     "自动折叠<br />
> nmap <silent> <F6> :Tlist<CR>        "映射快捷键F6，开启/关闭窗口

    WinManager 插件安装
> 下载地址：https://github.com/vim-scripts/winmanager <br />
> 解压后得到 doc 和 plugin 两个文件夹，将里面的内容复制到 vim 的对应文件夹中 <br />
> 在vimrc中添加设置 WinManager 的设置：<br />
> let g:winManagerWindowLayout='FileExplorer|TagList' <br />
> let g:winManagerWidth=25 <br />
> nmap wm :WMToggle<cr> <br />
> nmap <silent> <F7> :WMToggle<cr>      " 定义快捷键

    minibufexpl 插件安装
> 下载地址：http://www.vim.org/scripts/download_script.php?src_id=3640  <br />
> 将minibufexpl.vim复制到 vim 的 plugin 文件夹中  <br />
> 在vimrc中添加设置 minibufexpl 的设置：<br />
> let g:miniBufExplMapCTabSwitchBufs=1 <br />
> let g:miniBufExplMapWindowsNavVim=1 <br />
> let g:miniBufExplMapWindowNavArrows=1 <br />
