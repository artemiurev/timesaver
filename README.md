###Необходимые расширения для работы в VS Code


Это подборка минимально необходимых расширений для быстрого начала работы в Visual Studio Code. 
В проекте представлены подборки расширений для работы:
* Основное и самое необходимое - Essentials
* HTML
* Git


###Для кого будет полезно?
- - -
Начинающим программистам эта подборка будет полезна и сэкономит время на поиск и установку необходимых расширений.


###Как использовать?
- - -

* Откройте Visual Studio Code.
* Перейдите в раздел extensions `Shift+Cmd+X` и наберите в поиске `pack-essentials`, `pack-html` или `pack-git`. 
* Установите нужное и занимайтесь программированием.

###Как использовать проект?
- - -
* Убедитесь что у вас установлен `Node.js`
* Установить `npm install -g @vscode/vsce yo`
* Установить зависимости `npm install`
* Собрать файлы пакетов `.vsix`  `npm run build`
* Используйте собранные файлы `extensions/*/*.vsix` для быстрой установки расширений из файлов `.vsix` [Подробнее как это сделать см. тут](https://code.visualstudio.com/docs/editor/extension-marketplace#_install-from-a-vsix)
* Чтобы добавить новый проект, запустите из папки extensions `yo code`
```
$ yo code

     _-----_     ╭──────────────────────────╮
    |       |    │   Welcome to the Visual  │
    |--(o)--|    │   Studio Code Extension  │
   `---------´   │        generator!        │
    ( _´U`_ )    ╰──────────────────────────╯
    /___A___\   /
     |  ~  |     
   __'.___.'__   
 ´   `  |° ´ Y ` 

? What type of extension do you want to create? 
  New Extension (TypeScript) 
  New Extension (JavaScript) 
  New Color Theme 
  New Language Support 
  New Code Snippets 
  New Keymap 
❯ New Extension Pack 
  New Language Pack (Localization) 
  New Web Extension (TypeScript) 
  New Notebook Renderer (TypeScript) 
```
* Выбрать тип `New Extension Pack`
* В папке с созданным проектом добавьте в файле `package.json` секцию `extensionPack`
```
 "extensionPack": [ 
 	"publisher.extension-name",
 	"publisher.extension-1-name"
 ]
```
* В файле `package.json` определите свой `publisher`. Как его зарегистрировать см.тут [https://code.visualstudio.com/api/working-with-extensions/publishing-extension#create-a-publisher](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#create-a-publisher)


### Где найти еще больше расширений?

* [Visual Studio Code's Marketplace](https://marketplace.visualstudio.com/)
* Перейдите в раздел extensions `Shift+Cmd+X` в Visual Studio Code

**Всего доброго!**
