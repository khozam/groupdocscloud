---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Digitally Sign PDF Word Excel Images via cURL Commands for REST API"
head_description: "REST API to digitally sign popular document formats via cURL commands. Add signatures to PDF, Word, Excel, presentations &amp; image file formats."

############################# Header ############################
title: "Digitally Sign Documents with cURL"
description: "Use simple cURL commands to apply, verify & search e-signatures in various file formats with REST API. Supports variety of electronic signatures."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature Cloud for cURL"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-curl.png"
        product: "GroupDocs.Signature"
        platform: "Cloud for cURL"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/signature/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/signature/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      cURL is a free client-side URL transfer library that allows you to handle HTTP requests and responses in dealing with the GroupDocs.Signature Cloud REST API. The API allows you to create, verify and search different type of signature objects in a number of document formats. It provides a wide variety of signature options like putting signatures on a document, verify document and search signatures in it. The API supports HTTP requests and get responses in form of JSON or XML data. Hence, any language or platform which supports the HTTP requests and responses is capable of running the API.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by GroupDocs.Signature Cloud for cURL.
      
        left:
          enable: true
          icon: "fas fa-cogs"
          title: "Signature Options"
          content: |
            * Text
            * Image
            * Digital
            * Barcode
            * QR-Code            
        right:
          enable: true
          icon: "fas fa-crop"
          title: "Retrieve"
          content: |
            * Document Pages information
            * Document Properties
            * Supported formats list
            * Text and Digital
            * Barcode and QR-Code
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature Cloud supports electronically signing a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Supported Formats"
              content: |
                * **Word Processing**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, ODT, OTT, RTF, TXT
                * **Spreadsheet**: XLS, XLSX, XLSB, XLSM, ODS, OTS, CSV, TSV
                * **Presentation**: PPT, PPTX, PPTM, PPS, PPSX, PPSM, POTX, POTM, ODP, OTP

        right:
          enable: true
          table:
            # table loop
            - title: "Image and Other Formats"
              content: |
                * **Image**: BMP, DjVu, DNG, EMF, EPS, GIF, JP2, JPF, JPX, J2C, J2K, JPM, JPG, JPEG, ODG, PNG, PS, PSD, SVG, TIF, TIFF, WebP, WMF
                * **Portable**: PDF


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
    title: "Advanced Document Signature REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-list-alt"
        content: "Provide the list of supported document formats"

      # feature loop
      - icon: "fas fa-file-o"
        content: "Retrieve document pages information"

      # feature loop
      - icon: "fas fa-file-text-o"
        content: "Retrieve document properties"
      
      # feature loop
      - icon: "fas fa-check"
        content: "Verify Text and Digital signatures"

      # feature loop
      - icon: "fas fa-barcode"
        content: "Verify Barcode and QR-Code signatures"

      # feature loop
      - icon: "fas fa-retweet"
        content: "Cross-Platform Compatibility"
    
    more_feature:
      # more_feature_loop
      - title: "Get Started with Document Signing REST API"
        content: "It is easy to get started with GroupDocs.Signature Cloud as there is nothing to install. Simply create an account at GroupDocs Cloud and get your application information. Once you have the App SID & key, you are ready to give theGroupDocs.Signature Cloud REST API a try with any language - on any platform. Our e-Signing API for cloud allows you to e-sign a variety of documents with well-structured API calls."
      # more_feature_loop
      - title: "Supported Signature Types"
        content: "The API has flexible methods to add supported signatures to a number of supported document formats. For instance, the API provides methods to create Text Signature in Document Pages with different options of Text, location, alignment, font, margins, appearances and others in cURL command. Below mentioned is the simple example that shows how to retrieve supported file formats list using the cURL command."

      # more_feature_loop
      - title: "Supported file formats list - cURL"
        content: |          
          
          ```cURL
          curl -X GET "https://api.groupdocs.cloud/v2.0/signature/formats" -H "accept: application/json" -H "authorization: Bearer xxxxxx"
          ```
      # more_feature_loop
      - title: "Cloud based e-Signing API Features"
        content: |
                * Provide list of supported document formats
                * Obtain list of supported Barcode and QR-Code encode type names
                * Retrieve document properties like document size, creation and update dates, count of pages etc
                * Retrieve document pages information like pages count etc
                * Support signature for PDF documents
                * Support signature on Microsoft Documents formats like MSWord Documents, Excel Spreadsheets, PowerPoint Presentations
                * Support signature for Open Document Formats, HTML and many more
                * Verify documents for signatures
      # more_feature_loop
      - title: "Flexible Deployment Options"
        content: "Our RESTful electronic signature API is easy to understand, clearly documented and comes with SDKs and live examples for all major languages. For developers who prefer on-premises deployment, we also offer downloadable APIs for .NET, Java, PHP and many other platforms."
      # more_feature_loop
      - title: "Extensive File Type Support"
        content: "GroupDocs.Signature allows end users to sign documents literally in all common business formats, including PDF, Microsoft Word, Excel, PowerPoint, Rich Text format etc. "
      # more_feature_loop
      - title: "Cross-Platform Compatibility"
        content: "Being a RESTful API, GroupDocs.Signature Cloud can be used with any language or platform which supports HTTP requests and responses. You can also use GroupDocs.Signature Cloud with many third party storage providers including Amazon S3, Google Cloud, Google Drive and DropBox."
############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature Cloud also offers individual SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-net.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for .NET"
          link: "/signature/net"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-java.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SKD for Java"
          link: "/signature/java"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for PHP"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-php.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for PHP"
          link: "/signature/php"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Python"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-python.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Python"
          link: "/signature/python"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Ruby"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-ruby.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Ruby"
          link: "/signature/ruby"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Node.js"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-node.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Node.js"
          link: "/signature/nodejs"
        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Android"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_signature-for-android.png"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Android"
          link: "/signature/android"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---