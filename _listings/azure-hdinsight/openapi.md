---
swagger: "2.0"
x-collection-name: Azure HDInsight
x-complete: 1
info:
  title: HDInsightManagementClient
  description: the-hdinsight-management-client
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptActions/{scriptName}
  : delete:
      summary: Script Actions Delete
      description: Deletes a given persisted script action of the cluster.
      operationId: ScriptActions_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptactionsscriptname-delete
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: scriptName
        description: The name of the script
      responses:
        200:
          description: OK
      tags:
      - Script Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/executeScriptActions
  : post:
      summary: Clusters Execute Script Actions
      description: Begins executing script actions on the specified HDInsight cluster.
      operationId: Clusters_ExecuteScriptActions
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameexecutescriptactions-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters for executing script actions
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters Execute Script Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptActions
  : get:
      summary: Script Actions List
      description: Lists all persisted script actions for the given cluster.
      operationId: ScriptActions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptactions-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Script Actions
---