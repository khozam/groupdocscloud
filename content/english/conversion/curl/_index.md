---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Conversion"
product_tag: "conversion"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Convert Images PDF & Office Documents | cURL Commands for REST API"
head_description: "REST APIs for documents & images conversion via cURL commands. Convert between PDF, Microsoft Word, Excel, PPTX, Project, HTML, email and images."

############################# Header ############################
title: "Convert Document & Images using cURL"
description: "‎Document conversion using cURL commands for REST APIs. Quickly and reliably convert images and documents of any file format.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Conversion for Cloud for cURL"
        image: "/sdk/272x272/groupdocs_conversion-for-curl.webp"
        product: "GroupDocs.Conversion"
        platform: "cURL"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "https://docs.groupdocs.cloud/conversion/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/conversion/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Conversion Cloud lets you seamlessly convert your documents to literally any format you need. You can use cURL to send requests to the API. With this single API, you can convert back and forth between over 50 types of documents and images, including all Microsoft Office and OpenDocument file formats, PDF documents, HTML, CAD, raster images and many more. 
    tabs:
      enable: true   
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by GroupDocs.Conversion Cloud for cURL.

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Convert from documents
            * Convert to documents
            * Watermark pages
            * Password protect output

      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Conversion Cloud converts back and forth between a variety of documents and images.



        left:
          enable: true
          table:
            # table loop
            - title: "Convert From:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP, OTS, ODG
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX, POT
                * **Visio‎**: VSD, VDX, VSS, VSX, VST, VTX, VSDX, VDW, VSSX, VSTX, VSDM, VSTM, VSSM
                * **Project**: MPP, MPT, MPX
                * **Microsoft OneNote**: ONE
                * **Email**: MSG, EML, EMLX
                * **Fixed Layout**: PDF, XPS
                * **Web**: HTML, MHT, MHTML
                * **AutoCAD**: DXF, DWG, DWT, STL, DWF, IFC
                * **Image files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, DjVu, SVG, DNG, DIB, JPC, JPEG-LS
                * **Metafile**: WMF, EMF
                * **Other**: TXT, CSV, XML, DICOM, TEX, MOBI, EPUB, ICO

        right:
          enable: true
          table:
            # table loop
            - title: "Convert To:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP
                * **OpenDocument**:  XLS, XLSX, XLSM, XLSB, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Metafiles**: WMF, EMF
                * **Image Files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, SVG, DNG, PSD
                * **Other**: PDF, EPUB, TXT, HTML‎

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Conversion - Supported Operating Systems and Frameworks
        
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
    title: "Advanced Document Conversion API Features"

    feature:
      # feature loop
      - icon: "fas fa-retweet"
        content: "Convert across all common formats"

      # feature loop
      - icon: "fas fa-star"
        content: "Convert page by page or custom range of pages"

      # feature loop
      - icon: "fas fa-copy"
        content: "Watermark pages"
      
      # feature loop
      - icon: "fas fa-star"
        content: "Get high quality output files"

      # feature loop
      - icon: "fas fa-shield-alt"
        content: "Password protect output document"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on swagger collection"

      

    more_feature:
      # more_feature_loop
      - title: "Quick and Reliable Document Conversion"
        content: |
          GroupDocs.Conversion REST API has the capability to convert documents to any of the supported formats, with just a few lines of code.
      
      # more_feature_loop
      - title: "Quick conversion to any format with storage URL in output - cURL"
        content: |
          ```shell
          curl -X POST "https://api.groupdocs.cloud/v2.0/conversion" \
          -H "accept: application/json" \
          -H "authorization: Bearer TOKEN-HERE" \
          -H "Content-Type: application/json" \
          -d "{ \"StorageName\": \"First Storage\", \"FilePath\": \"/foldername/myfile.webp\", \"Format\": \"jpeg\", \"LoadOptions\": {}, \"ConvertOptions\": { \"FromPage\": 0, \"PagesCount\": 1, \"Pages\": [ 1 ] }, \"OutputPath\": \"/foldername\"}"
          ```

      # more_feature_loop
      - title: "Get Started in No Time"
        content: "With GroupDocs.Conversion Cloud API, you can start converting your files right away as there is no need to install anything. The API is clearly documented and comes with SDKs and live examples for all major languages. Our GroupDocs.Conversion SDKs along with working examples hosted at Github helps our users to get started in no time. "

      # more_feature_loop
      - title: "Security and Authentication"
        content: "The GroupDocs.Conversion Cloud API is secured and requires authentication. Users need to register at GroupDocs Cloud and get their app access key ID (appSID) and app secret access key. Authenticated requests require a signature and AppSID query parameters or OAuth 2.0 athrorization header."
      
      # more_feature_loop
      - title: "API Explorer"
        content: "The easiest way to try out GroupDocs.Conversion Cloud API right away in your browser is by using GroupDocs Cloud Web API explorer, which is a collection of Swagger documentation for the GroupDocs Cloud APIs. It also provides testing and interactivity to our API endpoint documentation."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Conversion Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_conversion-for-curl.webp"
          product: "GroupDocs.Conversion"
          platform: "cURL"
          link: "/conversion/curl/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_conversion-for-net.webp"
          product: "GroupDocs.Conversion"
          platform: ".NET"
          link: "/conversion/net/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_conversion-for-java.webp"
          product: "GroupDocs.Conversion"
          platform: "Java"
          link: "/conversion/java/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_conversion-for-php.webp"
          product: "GroupDocs.Conversion"
          platform: "PHP"
          link: "/conversion/php/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_conversion-for-python.webp"
          product: "GroupDocs.Conversion"
          platform: "Python"
          link: "/conversion/python/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_conversion-for-ruby.webp"
          product: "GroupDocs.Conversion"
          platform: "Ruby"
          link: "/conversion/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_conversion-for-node.webp"
          product: "GroupDocs.Conversion"
          platform: "Node.js"
          link: "/conversion/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_conversion-for-android.webp"
          product: "GroupDocs.Conversion"
          platform: "Android"
          link: "/conversion/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---