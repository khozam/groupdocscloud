---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Viewer"
product_tag: "viewer"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Render PDF Word Excel Outlook via cURL | Document Viewer REST API"
head_description: "REST APIs for Documents viewing and rendering via cURL commands. View PDF, images, Microsoft Word, Excel, PPTX, Visio, Project & 50+ file formats."

############################# Header ############################
title: "Simply use cURL to Render & View Documents"
description: "Exposes RESTful APIs to view and render business documents & attachments for supported file formats. Render as PDF, HTML, PNG or JPG image.
‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Viewer for Cloud"
        image: "/sdk/272x272/groupdocs_viewer-for-curl.webp"
        product: "GroupDocs.Viewer"
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
            - link: "https://docs.groupdocs.cloud/viewer/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/viewer/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Viewer Cloud for cURL allows you to seamlessly enhance your application with the capability to render a number of document formats. The API supports a variety of document formats and allows viewing a specific document in HTML, image, PDF or its original format with the flexibility to render the whole document, page by page or custom range of pages.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Viewer Cloud for cURL.

        left:
          enable: true
          icon: "fa fa-cogs"
          title: "Document Rendering"
          content: |
            * Word, Excel, Powerpoint
            * Visio, Project, Outlook, OneNote
            * OpenDocument
            * Images
            *CAD Drawing Image formats
            * PDF, XPS, Text, Web formats
            * Many more formats
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Rotating, Reordering
            * Watermarking pages
            * Rendering Attachments
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Viewer Cloud for cURL supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTX, XLTM
                * **PowerPoint:**  PPT, PPTX, PPS, PPSX, PPSM, PPTM, POTX, POTM
                * **Visio:** VSD, VSDX, VSDM, VST, VSTX, VSTM, VSS, VSSX, VSSM, VDX, VSX, VTX, VDW
                * **Project:** MPP, MPT
                * **Outlook:** MSG, EML, PST, OST
                * **OneNote:** ONE

            

        right:
          enable: true
          table:
            # table loop
            - title: "Images, Graphics & Diagrams"
              content: |
                * **OpenDocument:** ODT, OTT, ODS, OTS, ODP, OTP, ODG
                * **Fixed Layout:** PDF, XPS
                * **eBook:** EPUB, MOBI
                * **Image Files:** BMP, GIF, ICO, JPG, JPEG, PNG, PSD, SVG, TIF, TIFF, Webp, DjVu, DNG, DCM (DICOM)
                * **JPEG2000:** JP2, J2C, J2K, JPF, JPX, JPM
                * **CAD:** DGN, DWF, DWG, DXF, IFC, STL
                * **Markup:** HTML, MHT, MHTML, XML
                * **Metafile:** WMF, EMF, CGM
                * **Apple Mail:** EMLX
                * **PostScript:** PS, EPS
                * **Other:** RTF, TXT, TEX, CSV, TSV, PCL
                
      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Viewer Cloud for cURL - some of the supported languages and platforms.
        
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
    title: "Advanced Document Viewer REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Render documents as HTML5"

      # feature loop
      - icon: "fas fa-images"
        content: "Render documents as Image"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Rotate, reorder & watermark pages"
      
      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render documents as PDF"

      # feature loop
      - icon: "fas fa-paperclip"
        content: "Render document attachments"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

     

      

    more_feature:
      # more_feature_loop
      - title: "Quick and Reliable Request and Response"
        content: |
          The cloud based viewer API provides you all the supported file formats along with file extensions in a well formatted JSON response with just a few lines of code.
          Get Supported File Formats - cURL
          
          ```shell
          curl -X GET "https://api.groupdocs.cloud/v2.0/viewer/formats" \
          -H "accept: application/json" \
          -H "authorization: Bearer xxxxxxxxxx"
          ```
      # more_feature_loop
      - title: "Get Started with Document Viewing REST API"
        content: "It is easy to get started with GroupDocs.Viewer Cloud as there is nothing to install. Simply create an account at GroupDocs Cloud and get your application information. Once you have the App SID & key, you are ready to give the GroupDocs.Viewer Cloud REST API a try with any language - on any platform."

      # more_feature_loop
      - title: "Flexible Rendering of Documents"
        content: "GroupDocs.Viewer Cloud is a powerful document viewer REST API that allows you to display over 50 document formats in your applications. It allows document rendering for the whole document, page by page or custom range of pages."
       
       # more_feature_loop
      - title: "Language, Platform & Storage Independence"
        content: "GroupDocs.Viewer Cloud can not only be used with any language or platform which supports HTTP requests and responses, but it can also be used with many third party cloud storage providers including Amazon S3, Google Cloud, Google Drive and DropBox."

        # more_feature_loop
      - title: "Security and Authentication"
        content: "The GroupDocs.Viewer Cloud API is secured and requires authentication. Users need to register at GroupDocs Cloud and get their app access key ID and app secret access key. Authenticated requests require a signature and AppSID query parameters or OAuth 2.0 athrorization header."


        # more_feature_loop
      - title: "API Explorer"
        content: "The easiest way to try out GroupDocs.Viewer Cloud API right away in your browser is by using GroupDocs for Cloud Web API explorer, which is a collection of Swagger documentation for the GroupDocs Cloud APIs. It also provides testing and interactivity to our API endpoint documentation."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Viewer Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_viewer-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/viewer/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_viewer-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/viewer/net/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_viewer-for-java.webp"
          product: "GroupDocs.Viewer"
          platform: "Java"
          link: "/viewer/java/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_viewer-for-php.webp"
          product: "GroupDocs.Viewer"
          platform: "PHP"
          link: "/viewer/php/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_viewer-for-python.webp"
          product: "GroupDocs.Viewer"
          platform: "Python"
          link: "/viewer/python/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_viewer-for-ruby.webp"
          product: "GroupDocs.Viewer"
          platform: "Ruby"
          link: "/viewer/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_viewer-for-node.webp"
          product: "GroupDocs.Viewer"
          platform: "Node.js"
          link: "/viewer/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_viewer-for-android.webp"
          product: "GroupDocs.Viewer"
          platform: "Android"
          link: "/viewer/android/"
    

############################# Back to top ###############################
back_to_top:
  enable: true
---