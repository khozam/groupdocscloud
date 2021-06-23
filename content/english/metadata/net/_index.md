---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Metadata"
product_tag: "metadata"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Metadata Management Cloud SDK for PDF, Word, Excel & Images"
head_description: "C# .NET metadata API to read, write, edit, analyze, search, extract, remove, compare & export metadata of PDF Word Excel PPTX Outlook Audio Video & Images."

############################# Header ############################
title: ".NET Cloud SDK for Metadata Management"
description: "Add, modify, search, extract and remove metadata properties from documents and image file formats using metadata management cloud SDK and REST API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Metadata Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_metadata-for-net.webp"
        product: "GroupDocs.Metadata"
        platform: ".NET"

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
        link_download: "https://github.com/groupdocs-metadata-cloud/groupdocs-metadata-cloud-dotnet"
        link_learn: "https://docs.groupdocs.cloud/metadatacloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Metadata Cloud SDK for .NET allows users to extract and manage metadata properties from a variety of documents, images and other multimedia file formats within any type of .NET application.

      The metadata extraction API allows performing all useful metadata operations such as add, edit, retrieve and remove metadata from PDF, Microsoft Word, Excel spreadsheets, PowerPoint presentations, Outlook emails, Visio, OneNote, Project, audio, video, AutoCAD, archive, JPEG, BMP, PNG, TIFF and many more industry-standard file formats. You just need to define the search criteria and the metadata Cloud REST API will take care of the specified metadata operations within supported file formats.

      GroupDocs.Metadata Cloud is a REST API that offer extreme flexibility to programmers for using it with any language or platform that supports REST. It easily integrates with other cloud services to provide an ideal metadata management experience across web, mobile desktop or cloud platforms.


    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Metadata Cloud SDK for .NET only requires .NET Framework.

        right:
          enable: true
          icon: "fab fa-cubes"
          title: ".NET Framework"
          content: |
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Metadata Cloud supports a number of document formats.

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
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Metadata REST API while using your favorite language & platform.
        
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
      - title: "Add Metadata by Tag - .NET"
        content: |
          
          
          ```shell
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
              var configuration = new Configuration(MyAppSid, MyAppKey);
              var apiInstance = new MetadataApi(configuration);
              var fileInfo = new FileInfo
              {
                  FilePath = "documents/input.docx"
              };
              
              var now = DateTime.Now.ToString("MM-dd-yyyy hh:mm:ss");
              var options = new AddOptions
              {
                  FileInfo = fileInfo,
                  Properties = new List
                  {
                      new AddProperty
                      {
                          SearchCriteria = new SearchCriteriaWithoutValue
                          {
                              TagOptions = new TagOptions
                              {
                                  ExactTag = new Tag
                                  {
                                      Name = "Printed",
                                      Category = "Time"
                                  }
                              }
                          },
                          Value = now,
                          Type = "DateTime"
                      }
                  }
              };
              
              var request = new AddRequest(options);
              
              var response = apiInstance.Add(request);
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