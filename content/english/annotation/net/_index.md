---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: ".Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Document & Image Annotation Cloud SDK for PDF Word Excel HTML"
head_description: ".NET Cloud SDK & REST APIs for documents & images annotation. Add text and image annotation on PDF, images, HTML, Word, Excel, PPTX & emails."

############################# Header ############################
title: "Annotate Documents in C#"
description: ".NET Cloud SDK to communicate with REST APIs and build annotation tools for C# .NET applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Cloud"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-net.png"
        product: "GroupDocs.Annotation"
        platform: ".Net"

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
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-dotnet"
        link_learn: "https://docs.groupdocs.cloud/annotation/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud REST API for .NET allows you to programmatically work with business document annotation operations and develop tools using C# and other .NET technologies. The tools that you develop using our annotation SDK for .NET APIs, enable your end-users to annotate files of supported file formats, such as PDF, Microsoft Word, Excel, PowerPoint, Images and various other formats. Apply redactions, watermark overlays, sticky notes, pointers and text markups etc. The open-source SDK works as a wrapper for cross-platform .NET REST APIs. Apply annotations as drawings or text markups.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by our document annotation API for .NET.
      
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
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Annotation Cloud REST API while using your favorite language & platform.
      
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
        content: "GroupDocs.Annotation Cloud SDK for .NET allows you to utilize all the features of the GroupDocs.Annotation REST API which provides a number of ways to deal with the annotations. It not only allows retrieving annotations from documents but also adds (exports) annotation to a document and retrieves the resultant document as a stream. The below-mentioned example shows how easy is to import annotation using the SDK for .NET:"

      # more_feature_loop
      - title: "Import document annotations - C#"
        content: |
          
          ```java
            // Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            var configuration = new Configuration(AppSID, AppKey);
            var apiInstance = new AnnotateApi(configuration);

            // Set request.
            var request = new GetImportRequest()
            {
                filePath = "docs/document.docx"
            };

            var response = apiInstance.GetImport(request);
          ```
      # more_feature_loop
      - title: "Robust Set of Annotation Tools"
        content: "In GroupDocs.Annotation Cloud SDK for .NET, support for two primary annotation types is available. Each annotation type then further has numerous sub-types. The two primary types are; drawing based annotations and text-based annotations or markups.

        Text-based annotations are used to add comments to text selections, hide confidential text by redaction, apply underlines or strikethroughs to mark text, and stick notes to rich text.

        Whereas, graphical annotations are used to highlight area with rectanlgular shape and add notes to it, hide classified image or text, pick particular point within document and apply notes to it, drop arrow to an object to point towards it, draw lines and shapes, apply text-based watermarks, and distance based annotations."

      # more_feature_loop
      - title: "Easy Integration"
        content: "Integration of GroupDocs.Annotation Cloud SDK in to your C# or other .NET based applications is pretty easy and straight-forward. Simply create an account at GroupDocs.Cloud and get the App SID & App Key and you are good to go."

      # more_feature_loop
      - title: "Easy Customization"
        content: "Our Annotation SDK for .NET is open-source, and has an MIT license. GroupDocs.Annotation Cloud SDK is reliable, scalable and fully tested toolkit. So you can use it and even customize it as per your requirements free of charge."
      # more_feature_loop
      - title: "Interactive API Explorer"
        content: "Check our annotation API right now in your browser using Swagger based API explorer that lists all the features of GroupDocs.Annotation Cloud API for .NET. Provide your desired parameters to any feature and Try it out. You can visit our API Explorer now."
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for cURL"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-curl.png"
          product: "GroupDocs.Annotation"
          platform: "Cloud for cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for PHP"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-php.png"
          product: "GroupDocs.Annotation"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Python"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-python.png"
          product: "GroupDocs.Annotation"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Ruby"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-ruby.png"
          product: "GroupDocs.Annotation"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Node.js"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-node.png"
          product: "GroupDocs.Annotation"
          platform: "Node.js"
          link: "/annotation/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Android"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-android.png"
          product: "GroupDocs.Annotation"
          platform: "Android"
          link: "/annotation/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---