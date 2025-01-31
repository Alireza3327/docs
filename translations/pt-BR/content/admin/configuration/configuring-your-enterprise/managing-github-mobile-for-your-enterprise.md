---
title: Gerenciando o GitHub Mobile para a sua empresa
intro: 'You can decide whether people can use {% data variables.product.prodname_mobile %} to connect to {% data variables.product.product_location %}.'
permissions: 'Enterprise owners can manage {% data variables.product.prodname_mobile %} for a {% data variables.product.product_name %} instance.'
versions:
  ghes: '*'
type: how_to
topics:
  - Enterprise
  - Mobile
redirect_from:
  - /admin/configuration/configuring-your-enterprise/managing-github-for-mobile-for-your-enterprise
  - /admin/configuration/managing-github-for-mobile-for-your-enterprise
shortTitle: Gerenciar o GitHub Mobile
---

## Sobre o {% data variables.product.prodname_mobile %}

{% data variables.product.prodname_mobile %} allows people to triage, collaborate, and manage work on {% data variables.product.product_location %} from a mobile device after successful authentication. {% data reusables.mobile.about-mobile %} Para obter mais informações, consulte "[{% data variables.product.prodname_mobile %}](/get-started/using-github/github-mobile)".

You can allow or disallow people from using {% data variables.product.prodname_mobile %} to authenticate to {% data variables.product.product_location %} and access your instance's data. By default, {% data variables.product.prodname_mobile %} is{% ifversion ghes > 3.3 %} enabled for people who use {% data variables.product.product_location %}.{% else %} not enabled for people who use {% data variables.product.product_location %}. To allow connection to your instance with {% data variables.product.prodname_mobile %}, you must enable the feature for your instance.{% endif %}

{% ifversion ghes < 3.6 and ghes > 3.1 %}
{% note %}

**Note:** If you upgrade to {% data variables.product.prodname_ghe_server %} 3.4.0 or later and have not previously disabled or enabled {% data variables.product.prodname_mobile %}, {% data variables.product.prodname_mobile %} will be enabled by default. If you previously disabled or enabled {% data variables.product.prodname_mobile %} for your instance, your preference will be preserved upon upgrade. For more information about upgrading your instance, see "[Upgrading {% data variables.product.product_name %}](/admin/enterprise-management/updating-the-virtual-machine-and-physical-resources/upgrading-github-enterprise-server)."

{% endnote %}
{% endif %}

## Habilitar ou desabilitar {% data variables.product.prodname_mobile %}

{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.management-console %}
{% data reusables.enterprise_management_console.type-management-console-password %}
1. Na barra lateral esquerda, clique em **Celular**. !["Celular" na barra lateral esquerda para o console de gerenciamento de {% data variables.product.prodname_ghe_server %}](/assets/images/enterprise/management-console/click-mobile.png)
1. Em "GitHub Mobile", selecione ou desmarque **Habilitar aplicativos do GitHub Mobile**. ![Caixa de seleção para "Habilitar os aplicativos do GitHub móvel" no console de gerenciamento de {% data variables.product.prodname_ghe_server %}](/assets/images/enterprise/management-console/select-enable-github-mobile-apps.png)
{% data reusables.enterprise_management_console.save-settings %}
