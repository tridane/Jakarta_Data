Jakarta dengue (2007–2018) — CSVs derived from Prasetyowati et al. (2021)

Files and content
-----------------
1) jakarta_df_yearly_summary_2007_2018.csv
   - City-level totals per year: dengue cases (total and by age/sex) and incidence per 100,000.
   - Derived percentage columns (_pct) are computed from totals.
   - Source: table 1

2) jakarta_df_global_moransI_by_year.csv
   - Global Moran's I for village-level incidence by year; includes 2007–2018 overall row.
   - Source: table 2

3) jakarta_df_spatial_clusters_by_year.csv
   - For each year and cluster type (HH, LL, HL/LH outliers): number of cases, incidence per 10,000,
     number of villages in that cluster, and population at risk.
   - Source: table 3

4) jakarta_df_high_incidence_villages_2007_2018.csv
   - Villages named in the paper text as having highest cumulative incidence with values per 10,000.
   - Source: figure 5

5) jakarta_df_cluster_profile_summary.csv
   - Means/percentages for socio-ecological and demographic characteristics comparing HH vs LL clusters,
     with test statistics and p-values as reported.
   - Source: table 4

6) jakarta_df_cart_variable_importance.csv
   - Variable importance (percent) from the CART model separating HH vs LL clusters.
   - Source: table 5

7) jakarta_df_climate_correlations_summary.csv
   - Spearman's rho values for pairs explicitly reported in the text and Figure 4.
     (Pairs labeled "not significant" in the article are omitted due to lack of precise r.)
   - Source: figure 4

Provenance and caveats
----------------------
- All numeric values are transcribed from the tables/figures and narrative text of the article.
- Some table images in the PDF had minor OCR artifacts; totals were cross-checked so that age- and sex-specific counts sum to yearly totals.