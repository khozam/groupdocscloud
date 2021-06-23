---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document & Image Annotation Cloud SDK for PDF Word Excel HTML"
head_description: "Document annotation Cloud SDK for Java. Use REST APIs to digitally annotate PDF, images, HTML, Word, Excel, presentations, CAD & email file formats."

############################# Header ############################
title: "Annotate Documents in Java with REST API"
description: "RESTful API to build online document & image annotation tools with support for text & image based annotation options. Let's annotate!"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_annotation-for-java.webp"
        product: "GroupDocs.Annotation"
        platform: "Java"

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
        link_download: "https://purchase.groupdocs.cloud/pricing"
        link_learn: "https://purchase.groupdocs.cloud/pricing"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud SDK for Java is a handy toolkit for developing business document annotator applications in Java. The solution allows applying annotations, sticky notes, watermark overlays, redactions, text replacements and markups to documents, presentations, emails, spreadsheets, PDF, images other file formats. Annotation SDK works as a wrapper for the Java RESTful APIs and makes application cross-platform compatible. Our Annotation API also works with all popular 3rd party cloud storage solutions.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by our document annotation API for Java.
      
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
          GroupDocs.Annotation set of SDK REST APIs is not dependent on your local operating system or ‎database. We offer our SDK APIs in numerous programming languages and with frequent new ‎additions.
      
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
        content: "GroupDocs.Annotation Cloud API provides a number of ways to deal with annotations. It not only allows retrieving annotations from documents, but also adds annotation to a document and retrieves the resultant document as stream. Following code snippet shows how you can quickly get the PDF version of any document."

      # more_feature_loop
      - title: "Generate PDF of Document Pages - Java"
        content: |
          
          ```java
            // Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
                
            Configuration configuration = new Configuration(appSID, appKey);
            AnnotateApi apiInstance = new AnnotateApi(configuration);

            // Create request object.
            GetPdfRequest request = new GetPdfRequest();
            request.setFilePath("docs"+ File.separator +"document.docx");

            // Executing api method.
            File response = apiInstance.getPdf(request);
          ```
      # more_feature_loop
      - title: "Robust Set of Annotation Tools"
        content: "GroupDocs.Annotation Cloud SDK for Java REST API, allows you to make use of various types of annotations. The primary types are; graphical annotation and text-based annotations.

        Text-based markups can be done thorugh adding text comments to selection, text redaction is supported to hide classified text. You can also highlight text with markups such as underlines and strikethroughs. Sticky notes can be added to rich text.

        Graphical annotation can be applied in the form of, adding notes to area highlighted with rectangle (Area Annotation), hide classified part of text or image (Area Redaction), apply notes to a specific point within the document (Point Annotation), arrows dropped to an object (Pointer/Arrow), drawing freehand shapes and lines (Polyline), add text-based watermark overlay (Watermark), and distance meaurement between any two objects in the document (Distance Annotation)."

      # more_feature_loop
      - title: "Easy Integration"
        content: "To integrate GroupDocs.Annotation Cloud SDK into your Java applications, just create an account at GroupDocs.Cloud to get App SID & App Key. No installation is required."

      # more_feature_loop
      - title: "Easy Customization"
        content: "GroupDocs.Annotation Cloud SDK for Java is open source and has an MIT license. Use it, and even customize it for no charges. Moreover, it is tested and out of the box running for a quick and reliable integration."
      # more_feature_loop
      - title: "Interactive API Explorer"
        content: "Provide desired parameters to our Swagger based interactive API explorer and try out various features of GroupDocs.Annotation Cloud API for Java in your browser. Please visit Annotation Cloud API explorer to see it in action."
      

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
          image: "/sdk/272x272/groupdocs_annotation-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_annotation-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_annotation-for-java.webp"
          product: "GroupDocs.Viewer"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_annotation-for-php.webp"
          product: "GroupDocs.Viewer"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_annotation-for-python.webp"
          product: "GroupDocs.Viewer"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_annotation-for-ruby.webp"
          product: "GroupDocs.Viewer"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_annotation-for-node.webp"
          product: "GroupDocs.Viewer"
          platform: "Node.js"
          link: "/annotation/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_annotation-for-android.webp"
          product: "GroupDocs.Viewer"
          platform: "Android"
          link: "/annotation/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---