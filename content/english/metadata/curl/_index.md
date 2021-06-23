---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Metadata"
product_tag: "metadata"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "GroupDocs.Metadata Cloud for cURL"
head_description: "Manipulate metadata properties from PDF, Word, Excel, Presentations, multimedia, images and metafiles using Cloud REST API."

############################# Header ############################
title: "Document Metadata Management using cURL"
description: "Manipulate metadata properties from PDF, Word, Excel, Presentations, multimedia, images and metafiles using Cloud REST API.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Metadata Cloud for cURL"
        image: "/sdk/272x272/groupdocs_metadata-for-curl.webp"
        product: "GroupDocs.Metadata"
        platform: "Cloud cURL"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/metadatacloud/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/metadatacloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Metadata Cloud for cURL allows metadata properties management and manipulation across all common business document formats. It communicates with GroupDocs.Metadata Cloud REST API to handle HTTP requests and responses for you to add, edit, search and remove metadata properties from PDF, Word, Excel, audio, video, Visio, metafiles, images and many other file formats.


    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Metadata Cloud for cURL:

        left:
          enable: true
          icon: "fas fa-wrench"
          title: "Advanced APIs"
          content: |
            * Add Metadata
            * Update Metadata
            * Extract Metadata
            * Search Metadata
            * Replace / Remove Metadata
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Working with Audio, Video & Other Formats"
          content: |
            * Manipulate Metadata of Multimedia File Types
            * Read/Update Metadata
            * Read Image Files Metatadata
            * Extract Metadata of Image Files
            * Replace Metadata of ZIP Archive Files
            * Manipulate Metadata OpenType Fonts
            * Read vCard File Types
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Metadata Cloud allows editing a a variety of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOT, DOTX, DOCM
                * **Excel:**  XLS, XLSX, XLSM, XLTM
                * **PowerPoint:** PPT, PPTX, POTM, POTX, PPTM, PPS, PPSX‎, PPSM‎
                * **Outlook:** MSG, EML
                * **OneNote:** ONE
                * **Visio:** VSD, VDX, VSDX, VSS, VSX
                * **Project:** MPP

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, ODS
                * **Portable**: PDF
                * **Photoshop**: PSD
                * **AutoCAD**: DWG, DXF
                * **Audio**: MP3, WAV
                * **Video**: AVI, MOV, QT, FLV
                * **Metafiles**: EMF, WMF
                * **vCard**: VCF‎, VCR
                * **Image**: JPG, JPEG, JPE, JP2, PNG, GIF, TIFF, WebP, BMP, DJVU, DJV, DICOM‎  
                * **OpenType Fonts**: OTF, OTC, TTF, TTC‎
                * **Others**: EPUB, ZIP, TORRENT, ASF

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Metadata Cloud for cURL - some of the supported languages and platforms.
        
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
    title: "Advanced Document Metadata REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Secured REST oriented Metadata Management API"

      # feature loop
      - icon: "fab fa-html5"
        content: "Supporting more than 60 popular file formats"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Ability to View/Add Metadata"
      
      # feature loop
      - icon: "fas fa-file-alt"
        content: "Retrieve & Remove Metadata from Documents and Images"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Perform Search & Modify Metadata Operations on Supported File Types"

      # feature loop
      - icon: "fas fa-folder"
        content: "Flexible and Easy to Integrate with any language or platform"

      

    more_feature:
      # more_feature_loop
      - title: "Extract Metadata by Property Value - cURL"
        content: |
          
          
          ```shell
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            curl -v "https://api.groupdocs.cloud/connect/token" \
            -X POST \
            -d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
            -H "Content-Type: application/x-www-form-urlencoded" \
            -H "Accept: application/json"
              
            // cURL example to join several documents into one
            curl -v "https://api.groupdocs.cloud/v1.0/metadata" \
            -X POST \
            -H "Content-Type: application/json" \
            -H "Accept: application/json" \
            -H "Authorization: Bearer " \
            -d "{
                "FileInfo": {
                    "FilePath": "documents\\input.docx",
                    "StorageName": ""
                },
                "SearchCriteria": {
                    "ValueOptions": {
                        "Value": "Microsoft Office Word",
                        "Type": "String"
                    }
                }
            }"
          ```
      # more_feature_loop
      - title: "Retrieve Hidden Data for Manipulation"
        content: |
          GroupDocs.Metadata for Java provides you a comprehensive way to get and delete hidden data from Microsoft Word, Excel and PowerPoint files. You can also do the same for PDF documents. Following list elaborates the sort of metadata you can access and manipulate through GroupDocs.Metadata for Java:  

          * Microsoft Word (Comments, Hidden Text, Merge Fields)
          * Microsoft Excel (Comments, Hidden Sheets)
          * Microsoft PowerPoint (Comments, Hidden Slides)
          * PDF Documents (Attachments, Annotations, Bookmarks, Form Fields)

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Metadata offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Metadata for cURL"
          image: "/sdk/272x272/groupdocs_metadata-for-curl.webp"
          product: "GroupDocs.Metadata"
          platform: "cURL"
          link: "/metadata/curl/"

        # solution loop
        - img_alt: "GroupDocs.Metadata for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-metadata-net.webp"
          product: "GroupDocs.Metadata"
          platform: ".NET"
          link: "/metadata/net/"

        # solution loop
        - img_alt: "GroupDocs.Metadata for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-metadata-java.webp"
          product: "GroupDocs.Metadata"
          platform: "Java"
          link: "/metadata/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---