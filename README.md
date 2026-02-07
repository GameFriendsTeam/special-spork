# Minecraft Plugin Maker

## Описание
Minecraft Plugin Maker представляет собой визуальный конструктор плагинов для Paper и Spigot. Программа позволяет создавать серверные плагины без написания Java-кода. Генерация Java-файлов выполняется на основе шаблонов. Формирование plugin.yml и сборка итогового JAR-файла выполняются с использованием встроенного JDK.

## Возможности
Создание нового проекта  
Редактирование элементов: Items, Blocks, Entities, Recipes, Trades, Trees, Plants, Dialogues, Animations  
Автоматическая генерация Java-кода  
Генерация plugin.yml  
Сборка плагина с использованием встроенного JDK  
Компиляция через javac  
Упаковка через jar  
Работа с ресурсами: текстуры, модели, звуки, локализация  
Графический интерфейс на основе WPF  

## Структура проекта
PluginsMinecraftMaker  
api — Paper API  
Common — общие утилиты  
Core — логика генератора  
resources — ресурсы проекта  
runtime — встроенный JDK  
templates — шаблоны Java-кода  
UI — интерфейс WPF  

## Архитектура

### Common
Logger  
Paths  
FileUtils  
JsonUtils  
PathUtils  
ValidationUtils  

### Core Managers
ItemManager  
BlockManager  
EntityManager  
RecipeManager  
TradeManager  
TreeManager  
PlantManager  
DialogueManager  
AnimationManager  
EventManager  
ApiManager  
BuildManager  
TemplateEngine  
ManagersCodeGenerator  

### Core Models
ItemModel  
BlockModel  
EntityModel  
RecipeModel  
TradeModel  
TreeModel  
PlantModel  
DialogueModel  
AnimationModel  
PluginModel  

### ProjectSystem
Загрузка и сохранение проекта  
Управление структурой проекта  

## Шаблоны
templates/items/item.template  
templates/blocks/block.template  
templates/entities/entity.template  
templates/events/event.template  
templates/recipes/recipe.template  
templates/command.template  
templates/listener.template  
templates/main.template  
templates/plugin.yml.template  

## Процесс генерации
Создание проекта  
Заполнение данных элементов  
Генерация Java-файлов через ManagersCodeGenerator  
Подстановка данных в шаблоны через TemplateEngine  
Компиляция и упаковка через BuildManager  
Получение итогового plugin.jar  

## Лицензия
пока не определена.

## Контрибьютинг
Pull-request приветствуются. Возможны расширения функциональности, добавление новых менеджеров, улучшение интерфейса и оптимизация генерации.
