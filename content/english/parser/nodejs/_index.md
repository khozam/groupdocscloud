---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Parser"
product_tag: "parser"
platform: "Nodejs"
platform_tag: "nodejs"

############################# Head ############################
head_title: "Parse Documents and Extract Data with Node.js"
head_description: "Parse documents by template and fetch plain and formatted text, markdown text, HTML tags, images and document information using Node.js."

############################# Header ############################
title: "Extract data from your documents with this REST API & Node.js Cloud SDK"
description: "Extract text, images, metadata and other data from 40+ document formats. Apply template to extract tables or specific data fields."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Parser Cloud SDK for Nodejs"
        image: "/sdk/272x272/groupdocs_parser-for-node.webp"
        product: "GroupDocs.Parser"
        platform: "Node.js"

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
      GroupDocs.Parser Cloud for Node.js is a wrapper around document data extraction REST API to parse over 50 document types. Extract text in various modes, extract images, parsing documents with predefined templates are the most popular features of GroupDocs.Parser Cloud API.
      The API supports password protected files and containers like ZIP archives, OST/PST mail data files, eBooks, markups, and PDF portfolios in your Node.js applications.
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
      - title: "Extract Formatted text from a Document"
        content: "GroupDocs.Parser Cloud API, provides several ways to extract text from documents. Following example shows how to extract formatted text from a document."

      # more_feature_loop
      - title: "Extract formatted text from a document - Node.js"
        content: |          
          
          ```Node.js
          // For complete examples and data files, please go to https://github.com/groupdocs-parser-cloud/groupdocs-parser-cloud-node-samples
          global.parser_cloud = require("groupdocs-parser-cloud");
    
          global.appSid = "XXXX-XXXX-XXXX-XXXX"; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
          global.appKey = "XXXXXXXXXXXXXXXX"; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
      
          global.parseApi = parser_cloud.ParseApi.fromKeys(appSid, appKey);
    
          let fileInfo = new parser_cloud.FileInfo();
          fileInfo.filePath = "words-processing/docx/formatted-document.docx";
    
          let options = new parser_cloud.TextOptions();
          options.fileInfo = fileInfo;
    
          let formattedTextOptions = new parser_cloud.FormattedTextOptions();
          formattedTextOptions.mode = "Markdown";
          options.formattedTextOptions = formattedTextOptions;
    
          let request = new parser_cloud.TextRequest(options);
          let response = await parseApi.text(request);
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
        - img_alt: "GroupDocs.Parser Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_parser-for-net.webp"
          product: "GroupDocs.Parser"
          platform: ".NET"
          link: "/parser/net"

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
   

############################# Back to top ###############################
back_to_top:
  enable: true
---