---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "PHP"
platform_tag: "php"

############################# Head ############################
head_title: "eSignature PHP SDK for Document Digital Signature REST API"
head_description: "Build tools with open-source PHP SDKs to create, embed, search and verify numerous types of digital signatures. Document signing REST APIs."

############################# Header ############################
title: "Digitally Secure Documents via PHP SDK"
description: "Business document signing RESTful APIs for PHP help you build tools to create, embed, search and verify numerous types of digital signatures."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature Cloud SDK for PHP"
        image: "/sdk/272x272/groupdocs_signature-for-php.webp"
        product: "GroupDocs.Signature"
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
      With GroupDocs.Signature Cloud SDK for PHP, we want to help you speed up the adoption of e-Signatures and facilitate the integration of our document signing cloud APIs into your workflows. The SDK allows you to utilize all the features provided by the REST API like creating, verifying and searching different types of signature objects in a number of document formats in a much simpler manner. It supports a wide variety of signature options like putting signatures on a document, verifies document and searches signatures in it. 
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by GroupDocs.Signature Cloud SDK for PHP.
      
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
      # feature loop
      - icon: "fas fa-search"
        content: "Search multiple signatures"
      # feature loop
      - icon: "fas fa-sign-in"
        content: "Add multiple signatures"
    
    more_feature:
      # more_feature_loop
      - title: "Digitally Sign a Multitude of Documents"
        content: "GroupDocs.Signature allows end users to sign documents literally in all common business formats, including PDF, Microsoft Word, Excel, PowerPoint, Rich Text format etc. Since the SDK is basically a PHP library for communicating with the API, you can sign all those formats using the SDK as well."
      # more_feature_loop
      - title: "Supported Signature Types"
        content: "Our e-Signature RESTful API supports the following signature types:"
        content: |
                * Text Signature
                * Image Signature
                * Barcode Signature
                * QR-Code Signature
                * Digital Signature
                * Stamp Signature
                "The API has flexible methods to add supported signatures to a number of supported document formats. For instance, the API provides methods to create Text Signature in Document Pages with different options of Text, location, alignment, font, margins, and appearances by using Signature Options Object data in the request body."
      # more_feature_loop
      - title: "A Flexible SDK for your Specific Needs"
        content: "GroupDocs.Signature Cloud SDK for PHP allows you to incorporate a number of features supported by our e-signing REST API in your application. The following is a list of operations that are currently supported by the SDK for PHP:"
        content: |
                * Provide list of supported document formats
                * Obtain list of supported Barcode and QR-Code encode type names
                * Retrieve document properties like document size, creation and update dates, count of pages etc
                * Retrieve document pages information like pages count etc
                * Support signature for PDF documents
                * Support signature on Microsoft Documents formats like MSWord Documents, Excel Spreadsheets, PowerPoint Presentations
                * Support signature for Open Document Formats, HTML and many more
                * Verify documents for signatures\
      # more_feature_loop
      - title: "Get the API Working Really Fast"
        content: "GroupDocs.Comparison Cloud API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API SDKs in many development languages in order to make it easier to integrate with us. If you use SDK, it hides the REST API calls and lets you use GroupDocs.Comparison Cloud API features in a native way for your preferred language."
     
############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature Cloud also offers individual SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature Cloud for cURL"
          image: "/sdk/272x272/groupdocs_signature-for-curl.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud for cURL"
          link: "/signature/curl"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_signature-for-net.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud SKD for .NET"
          link: "/signature/net"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_signature-for-java.webp"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_signature-for-python.webp"
          product: "GroupDocs.Signature"
          platform: "Python"
          link: "/signature/python"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_signature-for-ruby.webp"
          product: "GroupDocs.Signature"
          platform: "Ruby"
          link: "/signature/ruby"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_signature-for-node.webp"
          product: "GroupDocs.Signature"
          platform: "Node.js"
          link: "/signature/nodejs"
          
        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_signature-for-android.webp"
          product: "GroupDocs.Signature"
          platform: "Android"
          link: "/signature/android"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---