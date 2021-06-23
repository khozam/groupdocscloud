---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "GroupDocs.Watermark Cloud for cURL"
head_description: "curl document watermarking API – Generate, search & remove watermarks from documents: PDF, Word, Excel, presentations, Visio, email and image file formats."

############################# Header ############################
title: "GroupDocs.Watermark Cloud for cURL"
description: "Manage image and text watermarks on all popular document formats using cURL commands. Add, find & delete watermarks on any language or platform supporting REST."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Watermark Cloud for cURL"
        image: "/sdk/272x272/groupdocs_watermark-for-curl.webp"
        product: "GroupDocs.Watermark"
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
            - link: "https://wiki.groupdocs.cloud/watermarkcloud/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/watermarkcloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark Cloud for cURL efficiently communicates with GroupDocs.Watermark Cloud REST APIs to manage all HTTP requests and responses for you to manage watermarks on supported document formats. It supports all useful watermarking methods such as adding, searching, updating and removing watermarks from PDF, Microsoft Office Word, Excel worksheets, presentations, Visio diagrams and image formats. You can also manage text style, size, font, color and position of the watermarks inside the whole document or restrict it to specific range of pages.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Watermark Cloud for cURL.

        left:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Watermarks management 
            * Manipulation solution
            * Add text
            * Image watermarks
            * Search watermark in documents


        right:
          enable: true
          icon: "fab fa-html5"
          title: "Implementation"
          content: |
            * Manage watermarks properties with ease
            * Replace already added watermarks
            * Remove watermarks from documents
            * Search by Image Comparison
            * Work with Headers & Footers
            * Work with Background Images
            * Work with Attachments
            * Rasterize Pages
            * Apply Editing Restrictions
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Watermark Cloud allows editing a a variety of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel:** XLS, XLSX, XLT, XLSM, XLTX, XLTM
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, PPTM, POTX, POTM
                * **Visio:** VSD, VSDX, VSDM, VSTX, VSTM, VSS, VSSX, VSSM, VDX, VSX, VTX

            
                

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT
                * **Fixed Layout**: PDF
                * **Image Files**: BMP, GIF, JPG, JPEG, JP2, PNG, TIFF, WebP
                * **Other**: RTF

            

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Watermark Cloud for cURL - some of the supported languages and platforms.
        
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
    title: "Advanced watermark management API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Search and delete already added watermarks from supported file formats"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Add or Remove Watermark from a specific pages or whole document"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Find text or image-based watermarks inside the documents"
      
      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Manage formatting settings to manipulate watermarks"

      # feature loop
      - icon: "fas fa-folder"
        content: "Cloud REST API to be used with any language or platform"

      # feature loop
      - icon: "fas fa-lock"
        content: "Secured watermark management solution"

      # feature loop
      - icon: "fas fa-folder"
        content: "API explorer based on swagger collection"

      
    more_feature:
      # more_feature_loop
      - title: "Add Watermark to the Document using cURL"
        content: |
          
          
          ```shell
          curl -v "https://api.groupdocs.cloud/v1.0/watermark" \
            -X POST \
            -H "Content-Type: application/json" \
            -H "Accept: application/json" \
            -H "Authorization: Bearer " \
            -d "{
                "FileInfo": {
                    "FilePath": "documents\\sample.pdf",
                },
                "WatermarkDetails": [
                    {
                        "TextWatermarkOptions": {
                            "Text": "Watermark text",
                            "FontFamilyName": "Arial",
                            "FontSize": 20.0,
                            "ForegroundColor": {
                                "Name": "red"
                            },
                            "TextAlignment": "center"
                        },
                        "Position": {
                            "X": 0.0,
                            "Y": 0.0,
                            "Width": 0.0,
                            "Height": 0.0,
                            "HorizontalAlignment": "Center",
                            "RotateAngle": 0.0,
                            "ConsiderParentMargins": false,
                            "IsBackground": false
                        }
                    }
                ]
            }"
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for cURL"
          image: "/sdk/272x272/groupdocs_watermark-for-curl.webp"
          product: "GroupDocs.Watermark"
          platform: "cURL"
          link: "/watermark/curl/"

        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/sdk/272x272/groupdocs_watermark-for-net.webp"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"
        
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/sdk/272x272/groupdocs_watermark-for-java.webp"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---