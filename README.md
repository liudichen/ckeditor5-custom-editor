# @iimm/ckeditor5-editor-decoupled

This repository presents a CKEditor 5 editor build generated by the [Online builder tool](https://ckeditor.com/ckeditor-5/online-builder)
一个自用的自定义ckeditor5的editor构架

## 版本对应

本构建的版本与ckeditor5-xxx版本对应关系

```text
├── 1.x
│   ├── 1.0.0   35.3.0
│   ├── 1.1.0   36.0.1 Base64UploadAdapter
|── 2.x 36.0.1 SimpleUploadAdapter
```

## 构建内容

```javascript
Editor.builtinPlugins = [
  Alignment,
  Autoformat,
  AutoImage,
  Base64UploadAdapter | SimpleUploadAdapter,
  Bold,
  Essentials,
  FindAndReplace,
  FontBackgroundColor,
  FontColor,
  FontFamily,
  FontSize,
  GeneralHtmlSupport,
  Heading,
  Highlight,
  Image,
  ImageCaption,
  ImageTextAlternative,
  ImageInsert,
  ImageResize,
  ImageStyle,
  ImageToolbar,
  ImageUpload,
  Indent,
  IndentBlock,
  Italic,
  List,
  ListProperties,
  Paragraph,
  PasteFromOffice,
  RemoveFormat,
  Strikethrough,
  Table,
  TableCaption,
  TableCellProperties,
  TableProperties,
  TableToolbar,
  TextTransformation,
  TodoList,
  Underline,
  WordCount,
  IndentFirstLine,
  LineHeight,
  ParagraphSpacing,
  ClearEmptyParagraph,
  ClearSpaceCharacter,
  SoftBreakToEnter,
  QuickStyle,
  ConvertFullHalf,
  Outline,
  FormatPainter,
];

Editor.defaultConfig = {
  toolbar: {
    items: [
      'fontFamily',
      'fontSize',
      'fontColor',
      '|',
      'bold',
      'italic',
      'underline',
      'strikethrough',
      'outline',
      '|',
      'alignment',
      'indentFirstLine',
      'lineHeight',
      '|',
      'imageUpload',
      '|',
      'formatPainter',
      'findAndReplace',
      'removeFormat',
      'undo',
      'redo',
    ],
  },
  language: 'zh-cn',
  fontFamily: {
    options: [ '宋体', '仿宋', '微软雅黑', '幼圆', '等线', '黑体', '隶书', '楷体', 'Arial', 'Times New Roman' ],
    supportAllValues: true,
  },
  fontSize: {
    options: [
      { title: '小四', model: '12pt' },
      { title: '四号', model: '14pt' },
      { title: '小三', model: '15pt' },
      { title: '三号', model: '16pt' },
      { title: '小二', model: '18pt' },
      { title: '二号', model: '22pt' },
      { title: '小五', model: '9pt' },
      { title: '五号', model: '10.5pt' },
      { title: '小六', model: '6.5pt' },
      { title: '六号', model: '7.5pt' },
      { title: '小一', model: '24pt' },
      { title: '一号', model: '26pt' },
      { title: '小初', model: '36pt' },
      { title: '初号', model: '42pt' },
    ],
    supportAllValues: true,
  },
  indent: {
    supportAllValues: true,
  },
  htmlSupport: {
    allow: [
      {
        name: /^(p|span|img|table|tbody|thead|tfoot|tr|td|th|col|colgroup|b|strong|s|sub|sup|u|i|em|h[1-6]|figure)$/,
        attributes: { width: true, height: true },
        classes: false,
        styles: true,
      },
    ],
  },
  image: {
    resizeUnit: '%',
    resizeOptions: [{
      name: 'resizeImage:original',
      value: null,
      icon: 'original',
    },
    {
      name: 'resizeImage:25',
      value: '25',
      icon: 'small',
    },
    {
      name: 'resizeImage:50',
      value: '50',
      icon: 'medium',
    },
    {
      name: 'resizeImage:75',
      value: '75',
      icon: 'large',
    }],
    toolbar: [
      'imageStyle:inline',
      'imageStyle:block',
      'imageStyle:side',
      '|',
      'resizeImage:25', 'resizeImage:50', 'resizeImage:75', 'resizeImage:original',
    ],
  },
  table: {
    contentToolbar: [
      'tableColumn',
      'tableRow',
      'mergeTableCells',
    ],
  },
};
```
