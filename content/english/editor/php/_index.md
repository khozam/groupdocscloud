---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: "Php"
platform_tag: "php"

############################# Head ############################
head_title: "PHP Document Editor Cloud SDK – Edit Word Excel HTML & Presentations"
head_description: "PHP Cloud SDK to communicate with GroupDocs REST APIs for editing business documents formats.  Edit Microsoft Word, Excel, PPTX, HTML & XML files.‎"

############################# Header ############################
title: "Documents Editor REST API & PHP Cloud SDK"
description: "Cloud REST API to quickly edit all popular document formats in any type of PHP application without installing any external software.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud SDK for PHP"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_editor-for-php.png"
        product: "GroupDocs.Editor"
        platform: "PHP"

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
        link_download: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-php"
        link_learn: "https://docs.groupdocs.cloud/editor/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud SDK for PHP supports editing and manipulating a bunch of popular document file formats within PHP applications. Simply integrate GroupDocs.Editor Cloud SDK for PHP with GroupDocs.Editor Cloud REST API, upload supported document in any third-party WYSIWYG HTML editor, manipulate the document and save it back to the original document format without disturbing the appearance after editing. The PHP editor library supports a variety of document formats including Microsoft Word (DOC, DOCX, WordML), Excel (XLS, XLSX, SpreadsheetML), Presentations (PPT, PPTX), HTML, XML, TXT and OpenDocument.

      GroupDocs.Editor Cloud SDK for PHP is built as a layer on top of GroupDocs.Editor Cloud REST API that saves valuable development time by managing low-level requests and handling responses. The developers can focus on writing up the specific code only as needed in the project.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          SDK requires PHP 5.5 or later. It can run on any platform where this requirement can be met.

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
      - title: "Working with WordProcessing Documents - PHP"
        content: |
          
          ```php
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          $AppSid = ""; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
          $AppKey = ""; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
            
          $configuration = new GroupDocs\Editor\Configuration();
          $configuration->setAppSid($AppSid);
          $configuration->setAppKey($AppKey);
          
          $editApi = new GroupDocs\Editor\EditApi($configuration);
          $fileApi = new GroupDocs\Editor\FileApi($configuration);
          
          // The document already uploaded into the storage
          // Load it into editable state
          $fileInfo = new Model\FileInfo();
          $fileInfo->setFilePath("Spreadsheet/four-sheets.xlsx");        
          $loadOptions = new Model\SpreadsheetLoadOptions();
          $loadOptions->setFileInfo($fileInfo);
          $loadOptions->setOutputPath("output");
          $loadOptions->setWorksheetIndex(0);
          $loadResult = $editApi->load(new Requests\loadRequest($loadOptions));
          
          // Download html document
          $htmlFile = $fileApi->downloadFile(new Requests\downloadFileRequest($loadResult->getHtmlPath()));
          $html = file_get_contents($htmlFile->getRealPath());
          
          // Edit something...
          $html = str_replace("This is sample sheet", "This is sample sheep", $html);
          
          // Upload html back to storage
          file_put_contents($htmlFile->getRealPath(), $html);
          $uploadRequest = new Requests\uploadFileRequest($loadResult->getHtmlPath(), $htmlFile->getRealPath());
          $fileApi->uploadFile($uploadRequest);
          
          // Save html back to xlsx
          $saveOptions = new Model\SpreadsheetSaveOptions();
          $saveOptions->setFileInfo($fileInfo);
          $saveOptions->setOutputPath("output/edited.xlsx");
          $saveOptions->setHtmlPath($loadResult->getHtmlPath());
          $saveOptions->setResourcesPath($loadResult->getResourcesPath());
          $saveResult = $editApi->save(new Requests\saveRequest($saveOptions));
          
          // Done.
          echo "Document edited: " . $saveResult->getPath();
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