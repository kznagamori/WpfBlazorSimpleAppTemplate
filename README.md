# WpfBlazorSimpleAppTemplate
WPF Blazorシンプルアプリを作成するためのテンプレート

## 使用法

### テンプレートの取得

`https://github.com/kznagamori/WpfBlazorSimpleAppTemplate.git`をダウンロードして、任意のディレクトリに展開します。


### テンプレートのインストール

`dotnet new install .\WpfBlazorSimpleAppTemplate`

### WPF Blazorアプリプロジェクトの作成

`dotnet new wpf-blazor-simple -n <プロジェクト名>`

**例:** `dotnet new wpf-blazor-simple -n MyWpfBlazor`

### ターゲットの設定

csprjファイルのTargetFrameworkの設定をビルドを行うdotnet sdkのバージョンに合わせます。

```
<Project Sdk="Microsoft.NET.Sdk.Razor">

  <PropertyGroup>
    <TargetFramework>net8.0-windows</TargetFramework>
```

`net8.0-windows`もしくは、`net7.0-windows`が設定可能です。

### パッケージのインストール

プロジェクトディレクトリ内で以下のコマンドを入力して、パッケージのインストールを行います。

#### net8.0
```
dotnet add package Microsoft.AspNetCore.Components.WebView.Wpf
```

#### net7.0
```
dotnet add package Microsoft.AspNetCore.Components.WebView.Wpf --version 7.0.101
```

### ビルド

```
dotnet build
```

### リリースビルド

```
dotnet publish -c Release
```

