---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Parser"
product_tag: "parser"
platform: "PHP"
platform_tag: "php"

############################# Head ############################
head_title: "Parse Documents and Extract Data with PHP"
head_description: "Parse documents by template and fetch plain and formatted text, markdown text, HTML tags, images and document information using PHP."

############################# Header ############################
title: "Document Parsing REST API & PHP Cloud SDK"
description: "Automate your document processing with GroupDocs.Parser. Extract data from documents by template. Process invoices, orders, reports and export data easily."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Parser Cloud SDK for PHP"
        image: "/sdk/272x272/groupdocs_parser-for-php.webp"
        product: "GroupDocs.Parser"
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
      GroupDocs.Parser Cloud for PHP is a wrapper around document data extraction REST API to parse over 50 document types. Parsing documents with predefined templates is one of the most valuable features of GroupDocs.Parser Cloud API. It is very simple and easy to define templates and extract data from invoices or other kinds of typical documents.
      The API provides methods to extract images, extract text and metadata from almost all of the most common file formats. Along with the regular documents, you can use the supported features on password protected files and containers like ZIP archives, OST/PST mail data files, eBooks, markups, and PDF portfolios in your PHP applications.
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
      - title: "Get Supported Document Types - PHP"
        content: |          
          
          ```PHP
          require_once(__DIR__ . '/vendor/autoload.php');
          //TODO: Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
          $configuration = new GroupDocs\Parser\Configuration();
          $configuration->setAppSid("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX");
          $configuration->setAppKey("XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX");

          $infoApi = new GroupDocs\Parser\InfoApi($configuration); 
          try {
            $response = $infoApi->getSupportedFileFormats();

            foreach ($response->getFormats() as $key => $format) {
              echo $format->getFileFormat() . " - " .  $format->getExtension(), "\n";
            }
          } catch (Exception $e) {
            echo  "Something went wrong: ",  $e->getMessage(), "\n";
            PHP_EOL;
          }
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