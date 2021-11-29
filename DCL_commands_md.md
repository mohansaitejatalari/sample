{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "DCL_commands.md",
      "provenance": [],
      "collapsed_sections": [],
      "authorship_tag": "ABX9TyOYgOVa5aMaEKfF6sxhqEwa",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/mohansaitejatalari/sample/blob/main/DCL_commands_md.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "BO8FAXVeoWz-"
      },
      "source": [
        "#**DATABASE**\n",
        "\n",
        "A Database is a collection of data that is organized and structurally stored in a computer system.\n",
        "\n",
        "Databases are of two types **Relational** and **Non Relational** .\n",
        "\n",
        "**Relational** Databases use **TABLES** and store data in rows and columns whereas, **Non-Relational** Databases uses **FILE SYSTEM**.\n",
        "\n",
        "\n",
        "##Data Control Language(DCL) \n",
        "\n",
        "In Databases , in order to access and update data in any DB , one must have the access to do so. This access for a user can be given and taken back (controlled) using the ***Data Control Language*** commands. \n",
        "\n",
        "The two DCL commands are **GRANT** and **REVOKE**\n",
        "\n",
        "\n",
        "####***GRANT***\n",
        "\n",
        "* This command is used to grant some or all privileges to a user on a particular DB Table or entire Database.\n",
        "* It accompanies DDL and DML commands , controls access over a DB to different users.\n",
        "* DB adminstrators can give and deny access to users of a DB at any point of time.\n",
        "\n",
        "_Syntax:_\n",
        "\n",
        "> **GRANT Privilege_name ON Object_name TO User_name;**\n",
        "\n",
        "Here,\n",
        "> * Privilege_name corresponds to opeartions like CREATE , INSERT , UPDATE etc.\n",
        "> * Object_name may be any Table name.\n",
        "> * User_name is the name of user to whom the access is to be granted.\n",
        "\n",
        "Consider a scenario where a user named Contributor needs access to perform basic operations supported on a Database named GWOC.\n",
        "\n",
        "The command to give above  access is : \n",
        "> **GRANT ALL ON GWOC TO CONTRIBUTOR;**\n",
        "\n",
        "\n",
        "####***REVOKE***\n",
        "* This command is used to deny or restrict access to a user on a Database.\n",
        "* Revoke helps in taking back all the privileges given in past to a user.\n",
        "\n",
        "_Syntax:_\n",
        "> **REVOKE Privilege_name ON object_name FROM user_name;**\n",
        "\n",
        "\n",
        "From contributor in the above scenario the privieges can be denied as\n",
        "> **REVOKE ALL ON GWOC FROM CONTRIBUTOR;**\n",
        "\n",
        "This is all about DCL commands.\n",
        "\n",
        "\n",
        "\n"
      ]
    }
  ]
}