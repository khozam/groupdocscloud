---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: ".Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Document Editor Cloud SDK – Edit Word Excel Presentations HTML"
head_description: ".NET document editor Cloud SDK REST APIs to render Microsoft Office Word, Excel, PPTX, HTML, XML without MS Office installed.‎"

############################# Header ############################
title: "C# .NET Documents Editor SDK"
description: "Cloud REST API to edit Word processing documents, Excel Spreadsheets & Presentations. Open document in WYSIWYG editor, edit and save back to original format."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_editor-for-net.webp"
        product: "GroupDocs.Editor"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support-resources"
              text: "Resources"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-dotnet"
        link_learn: "https://docs.groupdocs.cloud/editor/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud SDK for .NET allows developers to easily perform document editing functionalities within any type of .NET based application by integrating it with GroupDocs.Editor Cloud REST API. The .NET editor SDK supports editing all popular industry standard document types without needing to install Microsoft Office or Open Office on the system. Simply upload the supported document (Microsoft Word, Excel spreadsheets, PowerPoint, TXT, HTML, XML) file formats in any third-party front-end WYSIWYG HTML editor of your choice using GroupDocs.Editor Cloud API, perform editing and convert it back to its original file format.

      Using document editing SDK – manipulate word processing documents as a whole or page by page. Manage font extraction operation to offer the same layout and appearance of the document after editing. It supports defining the index of currently edited worksheet while editing the multi-tabbed Excel spreadsheets. Developers can also fix any issues within URLs, formatting options, document structure or recognition of email addresses within XML files.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Editor Cloud SDK for .NET only requires .NET Framework.

        left:
          enable: true
          icon: "fas fa-align-left"
          title: "Editing Option"
          content: |
            * Edit in flow or parged mode
            * Multi-language document
            * Manage font extraction
            * Support tabbed spreadsheets
            * Memory usage optimization
        
        right:
          enable: true
          icon: "fas fa-sitemap"
          title: "Information Extraction"
          content: |
            * Document Type
            * Document Size
            * Page Count
            
        
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Editor Cloud supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, FlatOPC, ODT, OTT, RTF, WordML
                * **Microsoft Excel**: XLS, XLSX, XLT, XLSM, XLSB, XLTX, XLTM, XLAM, SXC, SpreadsheetML, ODS, FODS, DIF, DSV, CSV, TSV
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX, PPSM, PPTM, POT, POTX, POTM, ODP, OTP

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Plain Text**: TXT
                * **Markup**: HTML, XML

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Editor REST API while using your favorite language & platform.
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced Document Editor REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Integrates easily within any WYSIWYG editor"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Edit Word documents as a whole or define pages range"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Multi-tabbed spreadsheet editing is supported"
      
      # feature loop
      - icon: "fas fa-file-alt"
        content: "Optimized memory usage for large CSV or TSV files"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Extract document information (type, size, page count etc)"

      # feature loop
      - icon: "fas fa-folder"
        content: "Cloud REST API to be used with any language or platform"



      

    more_feature:
      # more_feature_loop
      - title: "Working with WordProcessing Documents - C#"
        content: |
          
          ```cs
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          var configuration = new Configuration(MyAppSid, MyAppKey);
          
          // Create necessary API instances
          var editApi = new EditApi(configuration );
          var fileApi = new FileApi(configuration );
          
          // The document already uploaded into the storage.
          // Load it into editable state
          var loadOptions = new WordProcessingLoadOptions
          {
              FileInfo = new FileInfo
              {
                  FilePath = "WordProcessing/password-protected.docx",
                  Password = "password"
              },
              OutputPath = "output"
          };
          var loadResult = editApi.Load(new LoadRequest(loadOptions));
          
          // Download html document
          var stream = fileApi.DownloadFile(new DownloadFileRequest(loadResult.HtmlPath));
          var htmlString = new StreamReader(stream, Encoding.UTF8).ReadToEnd();
          
          // Edit something...
          htmlString = htmlString.Replace("Sample test text", "Hello world");
          
          // Upload html back to storage
          fileApi.UploadFile(new UploadFileRequest(loadResult.HtmlPath,
              new MemoryStream(Encoding.UTF8.GetBytes(htmlString))));
          
          // Save html back to docx
          var saveOptions = new WordProcessingSaveOptions
          {
              FileInfo = loadOptions.FileInfo,
              OutputPath = "output/edited.docx",
              HtmlPath = loadResult.HtmlPath,
              ResourcesPath = loadResult.ResourcesPath
          };
          var saveResult = editApi.Save(new SaveRequest(saveOptions));
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Editor offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Editor for cURL"
          image: "/sdk/272x272/groupdocs_editor-for-curl.webp"
          product: "GroupDocs.Editor"
          platform: "cURL for Cloud"
          link: "/editor/curl/"
          # solution loop
        - img_alt: "GroupDocs.Editor for .NET"
          image: "/sdk/272x272/groupdocs_editor-for-net.webp"
          product: "GroupDocs.Editor"
          platform: ".NET"
          link: "/editor/net/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Java"
          image: "/sdk/272x272/groupdocs_editor-for-java.webp"
          product: "GroupDocs.Editor"
          platform: "Java"
          link: "/editor/java/"
          # solution loop
        - img_alt: "GroupDocs.Editor for PHP"
          image: "/sdk/272x272/groupdocs_editor-for-php.webp"
          product: "GroupDocs.Editor"
          platform: "Php"
          link: "/editor/php/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Python"
          image: "/sdk/272x272/groupdocs_editor-for-python.webp"
          product: "GroupDocs.Editor"
          platform: "Python"
          link: "/editor/python/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Ruby"
          image: "/sdk/272x272/groupdocs_editor-for-ruby.webp"
          product: "GroupDocs.Editor"
          platform: "Ruby"
          link: "/editor/ruby/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Node.js"
          image: "/sdk/272x272/groupdocs_editor-for-node.webp"
          product: "GroupDocs.Editor"
          platform: "Node.js"
          link: "/editor/nodejs/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Android"
          image: "/sdk/272x272/groupdocs_editor-for-android.webp"
          product: "GroupDocs.Editor"
          platform: "Android"
          link: "/editor/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---