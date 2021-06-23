---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Android"
platform_tag: "android"

############################# Head ############################
head_title: "Android Document Signature Cloud SDK for PDF Word Excel PPTX & Images"
head_description: "Add e-signatures to images and documents with Android Cloud SDK & REST API. eSign PDF, Word, Excel & presentations with numerous signature types."

############################# Header ############################
title: "Android SDK to e-Sign Documents"
description: "Electronically sign files & manage text, image, QR-code, stamp, digital and barcode signatures in android applications with simple usage of e-signing REST API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature Cloud SDK for Android"
        image: "/sdk/272x272/groupdocs_signature-for-android.webp"
        product: "GroupDocs.Signature"
        platform: "Cloud SDK for Android"

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
      GroupDocs.Signature Cloud SDK for Android is a REST oriented API for easy integration into existing Android ‎based eSign and digital signature programs. This signature SDK helps you speed up the development ‎by taking care of low-level details, such as request and response handling. Moreover, it provides you ‎with a handy collection of features to apply various types of signatures, such as, image signatures, ‎barcode signatures, QR-Code signatures, text-based signatures, digital and stamp signatures. This ‎customizable Android based signature SDK allows you to work with signatures in spreadsheets, ‎presentations, images, portable and simple files of supported formats.‎‎
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by GroupDocs.Signature Cloud SDK for Android.
      
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
          GroupDocs.Signature Cloud supports multiple types of electronic signatures. Following list displays eSignature supported file formats:

        left:
          enable: true
          table:
            # table loop
            - title: "Text, Stamp & Image Signatures"
              content: |
                * **Word**: DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF‎
                * **Excel**: XLS, XLSB, XLSM, XLSX, XLT, XLTM, XLTX
                * **PowerPoint**: POT, POTM, POTX, PPS, PPSM, PPSX, PPT, PPTM, PPTX
                * **OpenDocument**: ODT, ODP, ODS, OTT
                * **Image**: JPG, PNG, BMP, GIF, TIFF
                * **Portable**: PDF
            # table loop
            - title: "Digital Signature"
              content: |
                * **Word**: DOC, DOCM, DOCX, DOT, DOTM, DOTX
                * **Excel**: XLS, XLSB, XLSM, XLSX, XLT, XLTM, XLTX
                * **PowerPoint**: PPTM, PPTX
                * **OpenDocument**: ODT
                * **Portable**: PDF

        right:
          enable: true
          table:
            # table loop
            - title: "Barcode Signature"
              content: |
                * **Word**: DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF‎
                * **Excel**: XLS, XLSB, XLSM, XLSX, XLT, XLTM, XLTX
                * **PowerPoint**: POT, POTM, PPSX, PPTX
                * **OpenDocument**: ODT, ODP, ODS, OTT
                * **Image**: JPG, PNG, BMP, GIF, TIFF
                * **Portable**: PDF
            # table loop
            - title: "QR-Code Signature"
              content: |
                * **Word**: DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF‎
                * **Excel**: XLS, XLSB, XLSM, XLSX, XLT, XLTM, XLTX
                * **PowerPoint**: PPTM, PPTX
                * **OpenDocument**: OTT
                * **Image**: JPG, PNG, BMP, GIF, TIFF
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
        content: "Get list of supported document formats"

      # feature loop
      - icon: "fas fa-barcode"
        content: "Fetch List of Supported Encode Type Names for Barcode and QR-Code"

      # feature loop
      - icon: "fas fa-file-text-o"
        content: "Retrieve Document Information from File or Provided URL"
      
      # feature loop
      - icon: "fas fa-pencil"
        content: "Apply Signature to a Document using File Name or at Specified URL"

      # feature loop
      - icon: "fas fa-align-right"
        content: "Apply Background Brush & Text Alignment to Text Signatures"

      # feature loop
      - icon: "fas fa-retweet"
        content: "Verify Text and Digital Signatures for PDF, Word and Excel Documents using File or via URL"
      # feature loop
      - icon: "fas fa-unlock-alt"
        content: "Verify Barcode and QR-Code Signatures for all Supported Document Formats‎ using File or via URL"
      # feature loop
      - icon: "fas fa-search"
        content: "Search Digital Signatures in PDF Files, Spreadsheets and Word Documents‎ in File or via URL"
      # feature loop
      - icon: "fas fa-binoculars"
        content: "Search Barcode and QR-Code Signatures in all Supported Document Formats‎ in File or via URL"
      # feature loop
      - icon: "fas fa-plus"
        content: "Add & Verify Multiple Signatures to Document using File Name or Provided URL"
      # feature loop
      - icon: "fas fa-file-text"
        content: "Search Multiple Signatures in a Document using its File Name or Provided URL"
      # feature loop
      - icon: "fas fa-check"
        content: "Try it with Interactive API Explorer"
    
    more_feature:
      # more_feature_loop
      - title: "Get Document Information"
        content: "GroupDocs.Signature Cloud SDK for Android makes it very easy to work with eSignatures. In addition to applying digital signatures you can also manipulate document properties. Following example elaborates how to retrieve document information of a DOCX file using Android:"
      # more_feature_loop
      - title: "Get Document Information using Android"
        content: |
          ```Android
          # Load the gem
            // Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            String appSid = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX";
            String appKey = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX";

            Configuration configuration = new Configuration(appSid, appKey);
            
            InfoApi infoApi = new InfoApi(configuration);

            try {            
              FormatsResult response = infoApi.getSupportedFileFormats();
                
              for (Format format : response.getFormats()) {
                System.out.println(format.getFileFormat());
              }
            } catch (ApiException e) {
              System.err.println("Exception");
              e.printStackTrace();
            }
              ```
      # more_feature_loop
      - title: "Set Background Brush for Stamp & Text Signatures"
        content: "Using GroupDocs.Signature Cloud SDK for Android, you can set background brush effects for your text ‎as well as stamp signatures. Currently, the SDK supports to apply 4 different types of brushes, which ‎include, Radial Gradient Brush, Linear Gradient Brush, Textured Brush, and Solid Brush.‎"
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
          platform: "Cloud SDK for Java"
          link: "/signature/java"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_signature-for-php.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for PHP"
          link: "/signature/php"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_signature-for-python.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Python"
          link: "/signature/python"

        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_signature-for-ruby.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for ruby"
          link: "/signature/ruby"
        # solution loop
        - img_alt: "GroupDocs.Signature Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_signature-for-node.webp"
          product: "GroupDocs.Signature"
          platform: "Cloud SDK for Node.js"
          link: "/signature/nodejs"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---