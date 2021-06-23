---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Parser"
product_tag: "parser"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Cloud SDK | Parser REST API | Data Extraction"
head_description: "Java document parser API to extract text, images, metadata &amp; encoding from databases, Word, Excel, presentations, PDF, email, EPUB and ZIP files."

############################# Header ############################
title: "Parse & Extract with REST API & Java SDK"
description: "Parse documents such as invoices, receipts or financial tables to extract text, images and metadata from 40+ popular document formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Parser Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_parser-for-java.webp"
        product: "GroupDocs.Parser"
        platform: "Java"

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
      GroupDocs.Parser Cloud for Java is a wrapper around document data extraction REST API to parse over 50 document types. Parsing documents with predefined templates is one of the most valuable features of GroupDocs.Parser Cloud API. It is very simple and easy to define templates and extract data from invoices or other kinds of typical documents.
      The API provides methods to extract images, extract text and metadata from almost all of the most common file formats. Along with the regular documents, you can use the supported features on password protected files and containers like ZIP archives, OST/PST mail data files, eBooks, markups, and PDF portfolios in your Java applications.
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
      - title: "Extract Images from a Document"
        content: "GroupDocs.Parser Cloud API, provides several ways to extract images from the documents. You can extract all the images from the whole document, extract images from the specific pages by setting pages range. Following example shows how to extract images from a document inside a container."

      # more_feature_loop
      - title: "Extract images from a PDF Portfolio - Java"
        content: |          
          
          ```Java
          // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
          String MyAppKey = "";
          String MyAppSid = "";

          Configuration configuration = new Configuration(MyAppSid, MyAppKey);
          ParseApi apiInstance = new ParseApi(configuration);

          FileInfo fileInfo = new FileInfo();
          fileInfo.setFilePath("pdf/PDF with attachements.pdf");
          fileInfo.setPassword("password");

          ContainerItemInfo containerItemInfo = new ContainerItemInfo();
          containerItemInfo.setRelativePath("template-document.pdf");

          ImagesOptions options = new ImagesOptions();
          options.setFileInfo(fileInfo);
          options.setContainerItemInfo(containerItemInfo);
    
          ImagesRequest request = new ImagesRequest(options);
          ImagesResult response = apiInstance.images(request);

          // For complete examples and data files, visit https://github.com/groupdocs-parser-cloud/groupdocs-parser-cloud-java-samples
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