---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Parser"
product_tag: "parser"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Cloud SDK | Parser REST API | Extract Text, Images & Data"
head_description: "C# .NET document parsing API to extract text, images, metadata & encoding from databases, PDF, Word, Excel, presentations, web, email, EPUB & zip file formats."

############################# Header ############################
title: "Parse & Extract with Cloud API & .NET SDK"
description: ".NET Parser SDK communicate with the REST API enabling you to build document parsing and data extraction tools on .NET platform."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Parser Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_parser-for-net.webp"
        product: "GroupDocs.Parser"
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
            - link: "https://docs.groupdocs.cloud/parser/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/parser/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Parser Cloud SDK facilitates .NET developers to parse any document to extract text, extract images and metadata within .NET based applications. SDK (REST API Client) is the easiest and quick way for the developer to speed up the development. This lets the developer focus on just to write the project-specific code and not to worry about the low-level details of making requests and handling the responses.
      Documents can be parsed by easy to use user-defined templates with data field definitions and table definitions. Then it's simple to extract data such as text fields, numbers, tables from the typical documents and even from containers like ZIP archives, OST/PST mail data files, eBooks, markups, and PDF portfolios.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document parser Cloud API.
      
        left:
          enable: true
          icon: "fas fa-list-ul"
          title: "Features"
          content: |
            * Parse documents
            * Parse document by template
            * Extract text
            * Extract images
            * Extract metadata
        right:
          enable: true
          icon: "fas fa-files-o"
          title: "Extract from Documents"
          content: |
            * Emails
            * eBooks
            * PDF files
            * PDF Portfolio
            * Files within ZIP archives
            * Text and Markup documents
            * Microsoft & OpenDocument Formats
      
      ## TAB TWO ##
      tab_two:
        description: |
          Document parser Cloud API supported formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word Processing**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Spreadsheets**: XLS, XLSX, XLSM, XLSB, XLT, XLTX, XLTM, XLA, XLAM
                * **Presentations**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POT, POTX, POTM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Other Formats"
              content: |
                * **OpenDocument Formats**: ODT, OTT, ODS, OTS, ODP, OTP
                * **Text**: TXT, RTF
                * **Markup**: HTML, XHTML, MHTML, MD, XML
                * **Portable Formats**: PDF
                * **Email**: PST, OST, EML, EMLX, MSG
                * **eBook Formats**: EPUB, FB2, CHM
                * **Other**: NUMBERS, CSV, ZIP


      ## TAB THREE ##
      tab_three:
        description: |
          Supported Operating Systems and Frameworks
      
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
    title: "Document Parser REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-files-o"
        content: "Parse PDF, word processing documents, spreadsheets & presentations"

      # feature loop
      - icon: "fas fa-file"
        content: "Parse Microsoft Word, Excel, PowerPoint and OpenDocument template files"

      # feature loop
      - icon: "fas fa-file-text"
        content: "Parse Macro-Enabled document & templates for MS Word, Excel & PowerPoint"
      
      # feature loop
      - icon: "fas fa-file-text-o"
        content: "Extract text content from the whole document"

      # feature loop
      - icon: "fas fa-file-image-o"
        content: "Extract text and images from specific pages"

      # feature loop
      - icon: "fas fa-font"
        content: "Extract formatted text by setting extraction mode"

      # feature loop
      - icon: "fas fa-file-archive-o"
        content: "Extract text from the documents in ZIP archives or Emails"

      # feature loop
      - icon: "fas fa-envelope-o"
        content: "Retrieve documents from Emails, PDF portfolios & MS Outlook storages"

      # feature loop
      - icon: "fas fa-files-o"
        content: "Get document page count and other information"
    
    more_feature:
      # more_feature_loop
      - title: "Extract Text from a Document by Page Number Range"
        content: "GroupDocs.Parser Cloud API, provides sevelral ways to extract text from the documents. You can extract only text, extract formatted text by setting extraction modes, extract from the specific pages by setting pages range. Following example shows how to extract text from a PDF document by setting page range."

      # more_feature_loop
      - title: "Parse PDF document to extract text from specific pages - C# .NET"
        content: |          
          
          ```.NET
          // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
            string MyAppKey = "";
            string MyAppSid = "";

            var configuration = new Configuration(MyAppSid, MyAppKey);

            var apiInstance = new ParseApi(configuration);
            var fileInfo = new FileInfo
            {
            FilePath = "directory/document.pdf"
            };

            var options = new TextOptions
            {
            FileInfo = fileInfo,
            StartPageNumber = 1,
            CountPagesToExtract = 2
            };

            var request = new TextRequest(options);
            var response = apiInstance.Text(request);

            // For complete examples, visit https://github.com/groupdocs-parser-cloud/groupdocs-parser-cloud-dotnet-samples
              ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Parser Cloud also offers individual document parsing SDKs for other languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Parser Cloud for cURL"
          image: "/sdk/272x272/groupdocs_parser-for-curl.webp"
          product: "GroupDocs.Parser"
          platform: "Cloud for cURL"
          link: "/parser/curl"

        # solution loop
        - img_alt: "GroupDocs.Parser Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_parser-for-java.webp"
          product: "GroupDocs.Parser"
          platform: "Java"
          link: "/parser/java"

        # solution loop
        - img_alt: "GroupDocs.Parser Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_parser-for-php.webp"
          product: "GroupDocs.Parser"
          platform: "PHP"
          link: "/parser/php"

        # solution loop
        - img_alt: "GroupDocs.Parser Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_parser-for-python.webp"
          product: "GroupDocs.Parser"
          platform: "Python"
          link: "/parser/python"

        # solution loop
        - img_alt: "GroupDocs.Parser Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_parser-for-ruby.webp"
          product: "GroupDocs.Parser"
          platform: "Ruby"
          link: "/parser/ruby"

        # solution loop
        - img_alt: "GroupDocs.Parser Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_parser-for-node.webp"
          product: "GroupDocs.Parser"
          platform: "Node.js"
          link: "/parser/nodejs"
   

############################# Back to top ###############################
back_to_top:
  enable: true
---