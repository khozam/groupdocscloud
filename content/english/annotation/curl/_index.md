---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Annotate Document & Images with cURL Commands for Cloud REST API"
head_description: "REST APIs for documents annotation via cURL commands to easily annotate PDF, images, Microsoft Word, Excel, PPTX, Visio, Project & 50+ file formats."

############################# Header ############################
title: "Annotate Documents with cURL"
description: "Communicate with REST API to add, remove and retrieve annotations. Retrieve a PDF version of any of the long list of supported document formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation Cloud for cURL"
        image: "/sdk/groupdocs_annotation-for-curl.webp"
        product: "GroupDocs.Annotation"
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
            - link: "https://docs.groupdocs.cloud/annotation/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/annotation/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud REST API helps you develop cross-platform document annotator. Build tools for annotating all common business documents and image file formats. Apply sticky notes, watermark overlays, pointers, drop arrows, redactions, and other types of graphic as well as text markups. Retrieve document information, render annotated documents to supported formats. Our Annotation RESTful API also supports 3rd part cloud storage, such as Amazon S3, Windows Azure, Dropbox etc.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by our document annotation API for cURL.
      
        left:
          enable: true
          icon: "fas fa-crop"
          title: "Figure Annotations"
          content: |
            * Area annotation
            * Point annotation
            * Area redaction
            * Polyline
            * Pointer/arrow
            * Watermark
            * Distance
        right:
          enable: true
          icon: "fas fa-file-alt"
          title: "Text Annotations"
          content: |
            * Annotation
            * Replacement
            * Redaction
            * Strikethrough / Underline
            * Typewriter
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation Cloud supports a number of document formats including almost all common business document and image file formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, RTF
                * **Excel**:  XLS, XLSX, XLSM, XLSB, CSV
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Visio**: VSD, VSDX, VSS, VST

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP
                * **Image Files**: BMP, PNG, JPG, JPEG, TIFF, TIF, GIF
                * **Fixed Layout**: PDF
                * **Web**: HTM, HTML
                * **Email**: EML
                * **CAD**: DWG, DXF


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
    title: "Advanced Document Annotation REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-thumbtack"
        content: "Add/remove graphic annotations & text markups"

      # feature loop
      - icon: "fas fa-info"
        content: "Retrieve document information such as metadata"

      # feature loop
      - icon: "fas fa-asterisk"
        content: "Fetch annotation data for supported file formats"
      
      # feature loop
      - icon: "fas fa-download"
        content: "Import/export annotation list of the document"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render annotated document to PDF"

      # feature loop
      - icon: "fas fa-upload"
        content: "Save resultant annotated document to storage & fetch its link"

      # feature loop
      - icon: "fas fa-tachometer-alt"
        content: "Support for multiple file formats & Cross-platform compatibility"

      # feature loop
      - icon: "fas fa-eye-slash"
        content: "Apply text redaction to the slide's content"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Apply annotations to Header/Footer area in Microsoft Word documents"
    
    more_feature:
      # more_feature_loop
      - title: "Work with Document Annotations"
        content: "GroupDocs.Annotation Cloud for cURL provides a number of ways to deal with annotations. It not only allows retrieving annotations from documents, but also adds (exports) annotation to a document and retrieves the resultant document as stream."

      # more_feature_loop
      - title: "Extract Document Annotations - cURL"
        content: |
          
          
          ```shell
          curl -X GET "https://api.groupdocs.cloud/v2.0/annotation?filePath=one-page.docx" \
          -H "accept: application/json" \
          -H "authorization: Bearer xxxxxx"
          ```
      # more_feature_loop
      - title: "Robust Set of Annotation Tools"
        content: "GroupDocs.Annotation Cloud for cURL supports a robust set of annotation types, which can primarily be divided into two categories; graphical annotations and text-based annotations. Both of these categories have further sub-categories of annotations and markups that you can use in your document annotation solutions.

        Text based annotations, include adding comments to various text selections, hiding text of choice by redaction, applying various text markups, e.g., underlines and strikethroughs, and adding sticky notes to rich text.

        On the other hand, graphical annotations include, area annotations to highlight area with rectangle in order to add notes, area redaction to hide classified text or image, point annotations to pick a point and apply notes to it, Pointer/arrow annotations to drop arrow for pointing towards an object within document, polyline annotation to draw freehand shapes and lines, watermark annotations to apply text-based watermark overlays, and distance annotations."

      # more_feature_loop
      - title: "Easy Integration"
        content: "Using the document annotation functionality of GroupDocs.Annotation Cloud with cURL is quite easy. Create an account at GroupDocs.Cloud to get the App SID & App Key. No type of installation is required to be done at the server or client end."
      

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
          image: "/sdk/groupdocs_annotation-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/groupdocs_annotation-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Java"
          image: "/sdk/groupdocs_annotation-for-java.webp"
          product: "GroupDocs.Viewer"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for PHP"
          image: "/sdk/groupdocs_annotation-for-php.webp"
          product: "GroupDocs.Viewer"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Python"
          image: "/sdk/groupdocs_annotation-for-python.webp"
          product: "GroupDocs.Viewer"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Ruby"
          image: "/sdk/groupdocs_annotation-for-ruby.webp"
          product: "GroupDocs.Viewer"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
          image: "/sdk/groupdocs_annotation-for-node.webp"
          product: "GroupDocs.Viewer"
          platform: "Node.js"
          link: "/annotation/nodejs/"

        

############################# Back to top ###############################
back_to_top:
  enable: true
---